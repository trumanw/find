# ![](https://www.internalpositioning.com/guide/img/wifi-marker-darkgrey-small.png) FIND

[![Build Status](https://travis-ci.org/schollz/find.svg?branch=master)](https://travis-ci.org/schollz/find)
[![Version 2.3](https://img.shields.io/badge/version-2.3-brightgreen.svg)](https://www.internalpositioning.com/guide/development/)
[![Github All Releases](https://img.shields.io/github/downloads/schollz/find/total.svg)](https://github.com/schollz/find/releases)
[![FIND documentation](https://img.shields.io/badge/find-documentation-blue.svg)](https://doc.internalpositioning.com/)
![Coverage](https://img.shields.io/badge/coverage-57%25-orange.svg)
[![Donate](https://img.shields.io/badge/donate-$1-brown.svg)](https://www.paypal.me/ZackScholl/1.00)
[![Join the chat at https://gitter.im/schollz/find](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/schollz/find?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![](https://raw.githubusercontent.com/schollz/find/master/static/splash.gif)](https://www.internalpositioning.com/)

**Keywords**: indoor GPS, WiFi positioning, indoor mapping, indoor navigation, indoor positioning

# About

**The Framework for Internal Navigation and Discovery** (_FIND_) allows you to use your (Android) smartphone or WiFi-enabled computer (laptop or Raspberry Pi or etc.) to determine your position within your home or office. You can easily use this system in place of motion sensors as its resolution will allow your phone to distinguish whether you are in the living room, the kitchen or the bedroom, etc. The position information can then be used in a variety of ways including home automation, way-finding, or tracking!

> Simply put, FIND will allow you to replace _tons_ of motion sensors with a _single_ smartphone!

The system is built on two main components - [a server](https://ml.internalpositioning.com/) and a fingerprinting device. The fingerprinting device ([computer program](https://github.com/schollz/find/releases/tag/v0.5) or [android app](https://play.google.com/store/apps/details?id=com.hcp.find)) sends the specified data to the machine learning server which stores the fingerprints and analyzes them. It then returns the result to the device and stores the result on the server for accessing via a web browser or triggering via hooks.

# TODO

- Abstract the key APIs.
- Re-organize the structure of projects through [cobra](https://github.com/spf13/cobra).
- Add instruments.
- Add new database interface for [etcd](https://github.com/coreos/etcd).
- Add new cache interface for [Redis](https://github.com/go-redis/redis).
- Docker compose launching support.
- Support Python classification like [scikit](http://scikit-learn.org/) via [google/grumpy](https://github.com/google/grumpy).
