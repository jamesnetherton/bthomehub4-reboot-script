bthomehub4-reboot-script
========================

Reboot the BT Home Hub 4 from the command line instead of using the nasty looking web interface. Useful for quick reboots or you can configure as a cron job for periodic restarts.

## Tested on
* Linux Mint 16 Petra
* BT Home Hub 4 (Type A), Software version 4.7.5.1.83.8.130.1.17 

## Dependencies
* cURL

## How it works
cURL is used to spoof the HTTP POST requests that would usually be made from the Home Hub web UI. A series of requests are made to the router in order to login and finally perform the reboot.

## Usage
To reboot your BT Home Hub 4 simply execute the reboot-router.sh script passing in your admin password. For example:

```bash
./reboot-router abc123
```
