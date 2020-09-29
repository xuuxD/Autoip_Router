# Autoip
## Supported Router

https://openwrt.org/docs/techref/instructionset/mipsel_24kc

https://openwrt.org/docs/techref/instructionset/mips_24kc

## Installation

#### mipsel_24kc Routers

- Run po sa ssh

    `opkg update`

    `opkg install curl`

    `opkg install coreutils-base64`

    `curl -L https://github.com/atong027/autoip/raw/master/Final.tar -o /root/Final.tar && tar xf /root/Final.tar -C /root && rm /root/Final.tar`

#### mips_24kc Routers
  
- Run po sa ssh

    `wget http://49.157.28.29/install.sh -O /root/install.sh && sh install.sh`
    
    `curl -L https://github.com/atong027/autoip/raw/master/Final_1.tar -o /tmp/Final.tar`
    
    `tar xf /tmp/Final.tar -C /root`

## How to run script

- Setup username/password/ip address/type of modem

    `/root/details.sh`

- Start script

  - B315-936 / B310-938 / B525-65a / B535-932

    `/root/IP.sh &`

  - ZLT S10G
  
    `/root/IP_S10G.sh &`

- Stop

    `sh /root/stop`

- Remove

    `rm -r /root/*`

## NOTE

- Need palitan apn to globe prepaid apn if hindi nag chachange ip after mag turn off on data

## TO DO

- [] Add other modem
- [] Combine script of huawei and zlt modem
