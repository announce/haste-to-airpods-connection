# haste-to-airpods-connection

## What's This?

Alfred Workflow to manage Bluetooth connection.

![Alfred Launcher](/../main/showcase/alfred-launcher.png?raw=true "airpods-connect")

## Prerequisite

Verified with:

* macOS v10.15.7
* Alfred Powerpack v4.3.3

Required package:

```shell
$ brew install bluetoothconnector
```

## Usage

1. Pair the target device with Mac at least once in advance
1. Spot the MAC address of your device with the command below:

```shell
$ BluetoothConnector
```

3. Download [haste-to-airpods-connection.alfredworkflow](https://github.com/announce/haste-to-airpods-connection/releases/download/1.0.0/haste-to-airpods-connection.alfredworkflow)
3. Click the downloaded file and import the workflow
3. Type `airpods-` on Alfred. You need to specify the MAC address so that the workflow will remember the one for later use. For instance, the MAC address would look like `00-03-93-a1-01-01`.

Here are the keywords available via Alfred:

* `airpods-status [MAC address]`: Show the current status of the target device.
* `airpods-connect [MAC address]`: Connect to the specified target device.
* `airpods-disconnect [MAC address]`: Disconnect from the target device.
