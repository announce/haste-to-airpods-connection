# haste-to-airpods-connection

## What's This?

Alfred Workflow to manage Bluetooth connection. 

In brief, this workflow provides several keywords to:

* connect to the target device and switch the audio output to the connected device
* disconnect from the current device

#### Typical Use Case Scenario 🎧

Type `airpods-connect` on Alfred:

![Alfred launcher](/../main/showcase/alfred-launcher.png?raw=true)

Then you will hear a machine voice saying "Connected" and get a notification showing the current audio volume:

![notification sample](/../main/showcase/notifications.png?raw=true)

## Prerequisite

Verified with:

* macOS Catalina (`10.15`), Big Sur (`11.3`)
* Alfred Powerpack v4.3.3

Required packages available via [Homebrew](https://brew.sh/):

```shell
$ brew install bluetoothconnector switchaudio-osx
```

## Install and Configuration

1. Download the latest **haste2.alfredworkflow** file from [**Releases**](https://github.com/announce/haste-to-airpods-connection/releases)
1. Click the downloaded file and import the workflow
1. Pair the target device with Mac at least once in advance
1. Spot the MAC address of your device with the command below:

```shell
$ BluetoothConnector
```

4. On the Alfred launcher, type `connect-airpods <YOUR_MAC_ADDRESS>` where `<YOUR_MAC_ADDRESS>` refers to the MAC address of your target device. You need to specify the MAC address only for the first time so that the workflow will remember the one for later use.
    * Tip: MAC address would look like `00-03-93-a1-01-01`.

## Usage

1. Just type `connect-airpods` on Alfred.

Here are the keywords available via Alfred:

* `airpods-status [MAC address]`: show the status of the specified device.
* `airpods-connect [MAC address]`: connect to the specified device.
* `airpods-disconnect [MAC address]`: disconnect from the current device.
* `connect-airpods`: alias to `airpods-connect`.
* `disconnect-airpods`: alias to `airpods-disconnect`.
