# Jabra Softphone example (BETA)

## About this example
This simple example shows how to add web based softphone support for a Jabra device using the [Jabra browser SDK](https://github.com/gnaudio/jabra-browser-integration).

The example softphone shows Jabra integration with the following features:
* Can run directly in Chrome with no additional installation steps apart from the [Jabra browser SDK](https://github.com/gnaudio/jabra-browser-integration).
* Support for outgoing and incomming calls.
* Support for mute and hold.
* Real audio experience using playback/loopback... You will only be talking to - and hearing - yourself in calls :-) 
* Extensive ringer with both Jabra device indication + sound in speakers.
* Two-way synchronization between softphone GUI and Jabra device when changing state. For example, when you select mute on either the softphone OR the Jabra device, both softphone and the Jabra device will be updated accordingly regardless of how it was initiated.
* Automatic selection of Jabra device microphone and speakers (user does not have to manually select the Jabra device in the browser and OS). This is important, as speaking using a device that is not selected is typically the number ONE support issue for most softphone users.

WARNING: This example is a BETA release - it has not been fully tested.

# Run the sample

TODO:

## Source code
For simplicity, the softphone example is written in plain javascript files (no modules) but we include the Jabra [typescript](https://www.typescriptlang.org/) declerations on top of most source files for better editor support. 

However, for non-trival softphones integrations we suggest you use [typescript](https://www.typescriptlang.org/), proper modularity and our npm module [@gnaudio/jabra-browser-integration](https://www.npmjs.com/package/@gnaudio/jabra-browser-integration).

The two most important source code files to look at are:
* ```softphone.stub.js``` that shows how to control a Jabra device from a fictive softphone.
* ```softphone.jabra.js``` that shows how to initialize the Jabra browser sdk and inform a softphone off key Jabra device events.

