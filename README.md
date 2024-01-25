# albion-overlay ![Status](https://img.shields.io/badge/status-%20active-brightgreen?style=flat&labelColor=gray) ![Version](https://img.shields.io/badge/beta-0.1.0-pink?style=flat&labelColor=salad)
An overlay program that will help you monitor cooldown of your friends abilities.
## :rocket: Project description. How it works?

Based on using Electron, I made an Overlay application that snaps one of its windows to the AlbionOnline-Client (just like the discord or teamspeak overlay you might have seen or used before does).

Overlay window lib link: https://www.npmjs.com/package/electron-overlay-window

frontend: React

backend: php

## 📦 What's going on under the box?
When connecting to a room, pressing a key combination, one of the additional worker windows (in the future this should happen in a different thread so that the interface does not freeze due to calculations), 

every second electron takes a screenshot of your screen, finds the circles of your abilities by coordinates, cuts them out , overlays an alpha channel, and sends it to the server.

Clients connected to your room receive data sent by you via websocket, generate an image based on a base64 string (*26-30Kb traffic per request*), and display it in the player’s panel.

## ⚠️ Violation policy ⚠️
The developer's response may concern you if you want to use this. Yes, SBI has openly stated that using any Overlay over an Albion window is prohibited. 

But at the same time, there were no incidents when players received a ban for using discord overlay. So, this program (literally **NOT A CHEAT**) cannot be detected by Easy-Anti cheat, 

does not use packages (which may be important during the proceedings), and does not provide information about enemy players. 

So you can use this with peace of mind, as long as you request access from the developer of course 😉

## 🔐 Privacy Policy
Yes, the software is to some extent spyware, as it processes what happens on your screen and sends this information over a secure (*https*) channel. 

The data is protected and is not used in any way on the server side. Also, scanning can be disabled by pressing the key combination 

**Ctrl+Shift+B** if you need to pause Overlay

## 🕵️‍♂️ 🛠️ Access to the Closed beta
Write applications to me in DM
Discord: an1medevka

