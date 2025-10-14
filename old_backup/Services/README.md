# [Services](../README.md)

## [Transmission Telegram Daemon](./transmission-telegram-d.service)

Unit file to run transmission telegram as a deamon.

Setup:

- Download the tar file from [transmission-telegram](https://github.com/pyed/transmission-telegram/releases)
- Extract the tar file and copy transmission-telegram file to your $PATH
- Now download [unit file](./transmission-telegram-d.service) and paste it in the target Directory.
- Enable the service `systemctl enable transmission-telegram-d.service`
- Start the service `systemctl start transmission-telegram-d`

| Target Directory |  Tested OS  |
| :--------------: | :---------: |
| `/usr/local/bin` | `Debian 12` |

Reference :
https://github.com/pyed/transmission-telegram

---
