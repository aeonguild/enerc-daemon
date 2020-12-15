<p align="center">
  <img src="image (1).png" width="250" style="border-radius: 10%;" title="hover text">
</p>

# Aeon daemon
 
AEON node for your Android phone. This is aeond packaged in an Android App.  

If you are looking for an android wallet, please see https://github.com/ivoryguru/aeonwallet

## Installation from github binaries

Make sure you enabled install from unknown sources in Android configuration (settings -> Security).

Then download the app in the release section. 

## Build it yourself

If you want to build the app yourself, the first thing is to get AEON on https://github.com/aeonix/aeon, then build binaries for arm64-v8a and armeabi, and then replace the compiled aeond binary under res/raw.

res/raw/aeond32 is the arm 32 bit compiled daemon, and res/raw/aeon64 is the 64 bit one.

Then import and build with android studio.  


## Phone requirements
A 64 bit processor with 10 Gb of storage is recommended to run on the mainnet blockchain.  


## Wallet connection
When the node is synchronized and running, a wallet app can connect locally to check and process payements.
Running a node locally is much safer than using a public node.  


## About Monero
If you want to build this app for Monero, just replace aeon32 and aeon64 by their monero ones, and change ressources and name in MainActivity:copyBinaryFile. That's it!  

## Tips
If your phone gets pretty hot during synchronization, go to "settings" -> "Limit rate" and set a value around 50 kB/s. This will reduce CPU usage but will make synchronization slower....  

You can copy your local data.mdb blockchain file from your local PC after syncing the blockchain to your phone's download folder (or microSD card) and use the app to select that file for syncing to reduce the need to fully sync all blocks from 0 with your android device.

The application saves the blockchain within itsself. The app size will grow as the blockchain size increases.

### License

Licensed under the Apache License, Version 2.0.

http://www.apache.org/licenses/LICENSE-2.0
