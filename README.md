# bubble-cordova-push
Bubble.is cordova build with push notifications

This project is to help Bubble.is users so they can build their own Bubble.is mobile apps with push notifications.
The build can also be used as a foundation to add your own or new cordova plugins to a Bubble.is hybrid app build.

Our goal for this repo should be:
1. Push notification implementation with a pre build cordova setup having all bubble required setup and cordova plugins
2. Guidance / code of how to integrate push on the different platforms iOS/Android
3. Guidance / code of how to execute push notifications from Bubble serverside flows.
4. Handling of incoming payloads / data from push message to open correct view or information when it is opened
4.1 Modal form displaying payload data with subsequent javascript or function call out from the modal
4.2 Webview displaying URL from payload
4.3 Displaying loading overlay while executing local function call or javascript

Folder structure:
/bubble-serverside/ [Contains instructions and eventual code  
/cordova-project/ [Contains the cordova project itself]
/push-vendors/    [Contains vendor recommendations and any specific code / instructions for implementation of this vendor]


WARNING #1: if you contribute, never submit any of your signatures,keys or other sensitivity your own repository may contain after testing push messages, those files should be on the gitignore.
This repo needs to be maintained in terms of plugins required by the Bubble.is generated codebase. 

WARNING #2: I provide no warranty or take any responsibility whatsoever for breaking anything in your app or for this repo being stable enough for a mobile app in production. 
Even though I think and hope it will :)


Contributions needed: 
1. Someone to develop, test and give feedback
2. Someone to make a complete list of gitignores for a cordova build so that we exclude any private keys, signatures etc.
3. Someone to test this for iOS using their iOS push certificates.

To discuss or contribute please use the following forum thread to keep the whole community involved: 
https://forum.bubble.is/t/future-feature-regarding-push-notifications/1949


GETTING STARTED (Incomplete, just providing a sample to get started)
1. Change the namespace of your app in the /cordova-project/index.js (LINE #XXX)
2.1 FOR IOS
    Put your keys and signatures in files X Y Z , build with 
2.2 FOR ANDROID 
    Generate X Y Z, do Z Y X
