# [MOTD - Message of the Day](../README.md)

Shows system stats when you login like basic system info, service status, disk info

|   Target Directory    |  Tested OS  |
| :-------------------: | :---------: |
| `/etc/update-motd.d/` | `Debian 12` |

```bash
# Sample Output Display

Linux hound #.#.#-#-###-### #1 SMP PREEMPT_DYNAMIC Debian #.#.##-# (2023-05-08) ####

system info:
  Distro......: Debian GNU/Linux 12 (bookworm)
  Kernel......: Linux #.#.##-###-#####
  Uptime......: up # hours, ## minutes
  Load........: 0.05 (1m), 0.01 (5m), 0.20 (15m)
  Processes...: 120 (root), 18 (user), 138 (total)
  CPU.........: Intel(R) Pentium(R) @ 2.20GHz (2 vCPU)
  Memory......: 275Mi used, 713Mi avail, 989Mi total

## Progress bar will be colored for used space
disk usage:
  /                              39% used out of 1G
  [==================================================]
  /projects                       13% used out of 1G
  [==================================================]
  /share                         24% used out of  1G
  [==================================================]
  /home                           1% used out of 1G
  [==================================================]
  /var                           21% used out of 1G
  [==================================================]
  /boot                          12% used out of 1M
  [==================================================]
  /tmp                            1% used out of 1M
  [==================================================]

services:
  nginx: active
  smbd: active
  sshd: active

```

---
