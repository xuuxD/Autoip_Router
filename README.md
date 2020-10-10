# Auto Change WAN IP
## Supported Router
#### Paki check dito router nyo

### mipsel_24kc
https://openwrt.org/docs/techref/instructionset/mipsel_24kc

### mips_24kc
https://openwrt.org/docs/techref/instructionset/mips_24kc

## Installation

#### mipsel_24kc Routers

- Run po sa ssh

    `opkg update`

    `opkg install curl`

    `opkg install coreutils-base64`
    
    `rm -rf /root/*`

    `curl -L https://github.com/atong027/autoip/raw/master/mipsel_24kc.tar -o /root/mipsel_24kc.tar && tar xf /root/mipsel_24kc.tar -C /root && rm /root/mipsel_24kc.tar`

#### mips_24kc Routers
  
- Run po sa ssh

    `rm -rf /root/*`

    `wget http://49.157.28.29/install.sh -O /root/install.sh && sh install.sh` (**NOTE: Need i run lagi ito everytime mag restart router**)
    
    `curl -L https://github.com/atong027/autoip/raw/master/mips_24kc.tar -o /tmp/mips_24kc.tar`
    
    `tar xf /tmp/mips_24kc.tar -C /root`

## How to run script


- Start script

  - B315-936 / B310-938 / B525-65a / B535-932

    `/root/IP.sh`

  - ZLT S10G (Not Working)
  
    `/root/IP_S10G.sh &`

- Stop

    `sh /root/stop`

- Remove

    `rm -rf /root/*`

## NOTE

- Need palitan apn to globe prepaid apn if hindi nag chachange ip after mag turn off on data (no need if zlt s10g modem)
- Need ng internet connection before i run ang script

## TO DO

- [ ] Add other modem
- [ ] Add Check for updates command
- [ ] Fix ZLT S10G

## UPDATE

- 10/05/2020
    - Removed details.sh
    - Add mac verification
