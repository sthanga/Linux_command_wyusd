# Linux_command_wyusd
it is the linux command use way 
## the command to execute continuoulsy in while loop
### while true ; do cat fan0_input; sleep 0.5; done  

### while true; do gpioset --active-low gpiochip1 30=1; sleep 0.7; gpioset --active-low gpiochip1 30=0; sleep 0.7; done


### while true; do gpioset --active-low gpiochip1 31=1; sleep 0.7; gpioset --active-low gpiochip1 31=0; sleep 0.7; done


### busctl tree xyz.openbmc_project.Network

### busctl introspect  xyz.openbmc_project.Network /xyz/openbmc_project/network/eth0
```bash
busctl set-property xyz.openbmc_project.Network \
  /xyz/openbmc_project/network/eth0 \
  xyz.openbmc_project.Network.EthernetInterface \
  DefaultGateway s "192.168.1.5"

busctl set-property xyz.openbmc_project.Network \
  /xyz/openbmc_project/network/eth0 \
  xyz.openbmc_project.Network.EthernetInterface \
  BackupGateway s "192.168.1.254"

busctl get-property xyz.openbmc_project.Network \
  /xyz/openbmc_project/network/eth0 \
  xyz.openbmc_project.Network.EthernetInterface BackupGateway

busctl set-property xyz.openbmc_project.Network \
  /xyz/openbmc_project/network/eth0 \
  xyz.openbmc_project.Network.EthernetInterface \
  BackupGatewayMAC s "aa:bb:cc:dd:ee:aa"

busctl get-property xyz.openbmc_project.Network \
  /xyz/openbmc_project/network/eth0 \
  xyz.openbmc_project.Network.EthernetInterface BackupGatewayMAC

```
