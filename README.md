# react-native-packetzoom [![npm version](https://img.shields.io/npm/v/react-native-packetzoom.svg?style=flat)](https://www.npmjs.com/package/react-native-packetzoom)

React Native PacketZoom SDK for iOS + Android

![](http://i.imgur.com/GPEgdkT.png)


# Intro

At PacketZoom we designed a modern, UDP-based network protocol with mobile apps in mind. This enables faster downloads, reduced latency, efficient and reliable data transfers between your app and the cloud. In addition to speed, one of the advantages of PacketZoom is that it handles seamless transition between networks without interrupting ongoing sessions. This is a unique advantage of the PacketZoom protocol over HTTP/TCP stack in common use today. 

Today we're redefining how networking works for React Native apps, empowering them with PacketZoom SDK and our worldclass cluster of servers.

[Join The Rebellion](https://packetzoom.com/get-started.html)

# Installation

First, download the library from npm:

```
npm install react-native-packetzoom@latest --save
```

Then you must install the native dependencies: You can use `rnpm` (now part of `react-native` core) to
add native dependencies automatically then continue the directions below depending on your target OS.

   `$ react-native link`
   
React Native versions from 0.30 and above should work out of the box, we cannot guarantee that earlier than 0.30
will have smooth integration experience, it may require additional manual steps like `rnpm` for example.

## Javascript
```js

import Packetzoom from 'react-native-packetzoom'

Packetzoom.init('packetzoom-app-id', 'packetzoom-api-key')
```

You can sign up for free PacketZoom account here: https://packetzoom.com/get-started.html

From now on all your [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) requests will be accelerated
by PacketZoom. You can access all [network analytics](https://packetzoom.com/blog/introducing-http-optimizer-and-analytics-service.html) data on web dashboard when you login under your account.


## iOS

Drag PZSpeed.Framework from RNPacketZoom.xcodeproj to your app frameworks folder like shown bellow:

![](http://i.imgur.com/z71C8Nh.png)


Make sure you linking against it in Build Phases -> Link Binary with Libraries section

![](http://i.imgur.com/e6ftLfX.png)

## Android

No additional changes required for Android

Enjoy request speedups and uninterrupted network connections across all mobile and wifi networks
