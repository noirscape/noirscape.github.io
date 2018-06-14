---
layout: post
title: "Getting the Android SDK working under Arch Linux"
tags: [arch linux, android]
categories: guides
---

I for the past few months have been using the program Ionic to make an application. Disregarding the fact that I'm using typescript (think javascript but somehow more annoying to use), today I had to build my application into an APK. As I'm using Manjaro, I was trying to set up the Android SDK packages in the AUR, before quickly running into some issues. So here's a quick guide on how to get the Android SDK working under Arch based distros (Arch based since Manjaro is basically Arch without the pathological need to -Syu daily. No you do that weekly instead.)

## Step 0: Get an AUR helper

Okay so before I continue any further, you can do this entire installation _without_ using a helper. In fact, if you're not familiar with how Arch Linux packaging works, it might even be preferable to not use one, as learning what the various helpers _do_ is a rather essential part of using the AUR. [Here](https://wiki.archlinux.org/index.php/Arch_User_Repository#Installing_packages) is a great place to get you started. That said, a helper is recommended. Of all the various helpers out there, at the moment I recommend [pacaur](https://aur.archlinux.org/packages/pacaur/), although it's been deprecated for over 6 months now, it's the helper that provides pacman style syntax and functionally acts as a drop-in replacement for pacman (you can replace any guide that tells you to do "sudo pacman" somewhere with simply "pacaur".

The main reason you want to know what a helper does is in case one of the packages (or it's dependencies) break in the AUR. By far the most common cause for package breakage is usually not updating checksums, and knowing how to fix that and manually install the update is an incredible help.

## Step 1: Install the appropriate packages

Very simple. Just use your favorite helper to install the following packages (or use `makepkg`, whatever floats your boat really). This is pretty straightforward.

The packages you need are:

> android-sdk android-sdk-build-tools android-sdk-platform-tools android-platform

Optionally, if like me you are using Ionic, you'll also want to install `gradle`, but this is not an AUR package.

## Step 2: Set the environment variables

Add the following line to your bashrc/zshrc/etc:

> export ANDROID_HOME=/opt/android-sdk

## Step 3: Accept the licenses

This for me was the most annoying step, as this is not documented on the Arch Wiki, but on [StackOverflow](https://stackoverflow.com/q/39760172/4666756) but you'll need to do the following things.:

> # chmod -R 777 /opt/android-sdk
> # ./sdkmanager --licenses
> (type yes a couple times)

Afterwards it should work. As to why you set android-sdk to 777, it's because when I used ionic, gradle still had to download the Android SDK itself, and it lacked permissions to do that. There's probably a better solution, but this worked for me.

Hope it's useful to someone out there.
