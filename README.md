# iOS Keylogger (Educational PoC)

> **⚠️ For Educational & Research Purposes Only**
>Auther : Abdulrahman Al-Hakami

This project is a simple **keylogging PoC (Proof of Concept)** for iOS, demonstrating how user input can be captured and exfiltrated to a remote server over HTTP. It is designed to work on real iOS devices and is implemented using Swift + UIKit inside a SwiftUI wrapper.

## Features

- Simple UI with three fields:
  - Attacker IP address input
  - Keystroke (to send as HTTP Header)
  - Keystroke (to send in HTTP Body)
- Sends captured input to a remote server (`http://[IP]:8080/log`)
- Base64 encoding for transmitted data
- Compatible with real iOS devices (tested on iPadOS 15.5)

##  Purpose

This application is built as a **security research demo** to:

- Simulate basic keylogging behavior in iOS.
- Test how input can be sent externally via HTTP headers and bodies.
- Help bug bounty hunters or researchers test apps and systems against data exfiltration vectors.

It can be used to:
- Practice **network traffic interception** (with tools like Burp Suite, Wireshark)
- Simulate malicious behavior for **defensive testing**
- Demonstrate how apps might misuse `UITextField` data and export it silently

##  Installation

Download the `.ipa` file from the **[Releases](#)** section or [direct link](#) (replace with actual link).

Install using:
if you use macOS I suggest you use sideloadly with your apple ID iCloud 
link : https://sideloadly.io




```bash
ios-deploy --bundle ./iOS-keylogger1.ipa
