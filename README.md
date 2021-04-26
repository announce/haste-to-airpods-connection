# haste-to-airpods-connection

## What's This?

Alfred Workflow to manage Bluetooth connection.

![Alfred Launcher](/../main/showcase/alfred-launcher.png?raw=true "airpods-connect")

## Prerequisite

Verified with:

* macOS v10.15.7

Required package:

```shell
$ brew install bluetoothconnector
```

## Usage

1. You need to pair the target device with Mac at least once in advance.
1. Spot the MAC address of your device with the command below:

```shell
$ BluetoothConnector
```

3. For the 1st time, you need to specify the MAC address of the target device. The workflow will remember the provided MAC address for later use. The MAC address would look like `00-03-93-a1-01-01`.

Here are the keywords available via Alfred:

* `airpods-status [MAC address]`: Show the current status of the target device. If the MAC address is not specified, the workflow reuse the last provided one.
* `airpods-connect [MAC address]`: Connect to the specified target device. If the MAC address is not specified, the workflow reuse the last provided one.
* `airpods-disconnect [MAC address]`: Disconnect from the target device. If the MAC address is not specified, the workflow reuse the last provided one.
