# GL-AR750 - Release Notes

## V3.203 - Aug 3, 2021

- Firmware file: [openwrt-ar750-3.203-0701.bin](https://fw.gl-inet.com/firmware/ar750/v1/openwrt-ar750-3.203-0701.bin)

    SHA256: d54d2436d6e381737c4bdba7cfc429e536ad1720172e87d866d2668fe7bd7e3d

**OpenWrt Distribution:**

- Based on OpenWrt 19.07.7  (AR150,MIFI,AR300M,USB150,N300,AR750,AR750S,X750,E750,X1200,- XE300,MT300N-V2,MT1300,MV1000)
- Based on QSDK11  (B1300,S1300,AP1300)

**Security:**

- Fixed wolfSSL heap buffer overflow in RsaPad_PSS (CVE-2020-36177)
- Fixed netifd and odhcp6c routing loop on IPv6 point to point links (CVE-2021-22161)
- Fixed dnsmasq multiple vulnerabilities (CVE-2020-25681, CVE-2020-25682, CVE-2020-25683, CVE-2020-25684, CVE-2020-25685, CVE-2020-25686, CVE-2020-25687)
- Fixed mac80211 FragAttacks(CVE-2020-24586,CVE-2020-24587,CVE-2020-24588,CVE-2020-26139,CVE-2020-26140,CVE-2020-26141,CVE-2020-26142,CVE-2020-26143,CVE-2020-26144,CVE-2020-26145,CVE-2020-26146,CVE-2020-26147)
- Added times limit to password authentication

**New features:**

- Supported IPv6 ( Internet, OpenVPN, WireGuard )
- Supported WPA3 (AR150,MIFI,AR300M,USB150,N300,AR750,AR750S,X750,E750,X1200,XE300)
- Supported deleting offline clients
- Added warnings when uploading old version or three-party firmwares
- Added 2.4G WIFI and LTE working channel interference automatic avoidance(MIFI,X750,E750,X1200,XE300)
- Supported IGMP 
- Supported DLNA

**Hardware support:**

- Supported SPI nand GD5F1GQ5UEYIG

**Optimization:**

- Optimized client statistics function

**APP support:**

- Supported GL.iNet App

**Cloud support:**

- Supported Rtty SSH Access
- Supported Rtty HTTP Access
- Supported Ping tool
- Supported Traceroute tool
- Supported RS485 tool（X300B)

**Language:**

- Supported Russian

**Important bug fix:**

- Fixed speed limit function failure in some models
- Fixed tor initialization failure in some models
- Fixed the problem that when turn off the AP in MT300N-V2, the repeater won't auto-reconnect.
- Fixed the problem that when WireGuard's Allowed IPs are not set with global proxy address, router will be unable to access the internet. 
- Fixed the problem that MT1300 can't access internet when using StrongVPN.
- Fixed a BUG where the OpenVPN connection status was displayed incorrectly on the E750 LCD
- Fixed XE300 modem manual settings always being overwritten when reboot 
- Fixed DNS leakage when using OpenVPN and WireGuard
- Fixed other known issues.

---

## V3.105 - Dec 8, 2020

- Firmware file: [openwrt-ar750-3.105.bin](https://fw.gl-inet.com/firmware/ar750/v1/openwrt-ar750-3.105.bin)

    MD5: 214da2c1ddeb6369371b208bacf55d5f

**New features:**

- Supported traffic statistics in bridge mode
- Supported OpenVPN bridge
- Supported NextDNS personal ID
- File sharing supported closing LAN sharing and supports shared folder selection
- OpenVPN server supported CHACHA20-POLY1305 encryption
- OpenVPN server supported Authentication option setting
- WireGuard server supported local network access switch
- The modem supported QCM protocol, SMS forwarding, adding Auth, Proto, TTL, and other configuration options (MIFI, X750, E750, X1200)
- Supported MCU setting (E750)
- Supported AdGuardHome (S1300)

Software Upgrade:

- Openssl upgraded to 1.1.1d
- Openvpn upgraded to 2.5.0

Optimization:

- Optimized real-time traffic statistics and reduce CPU load
- Optimized MQTT
- Optimized 4G to WiFi speed (MIFI,X750,E750)
- Optimized the number of X1200 5G client connections

Language:

- Supported Russian
- Fixed the problem of incomplete and inaccurate translation of some languages

UI:

- Added VPN status indicator icon to the navigation page
- Added quick navigation to WireGuard client commercial configuration
- Removed the import method with JSON format in WireGuard client 

Important bug fix:

- Fixed the problem that AdGuardHome cannot be upgraded
- Fixed MV1000 memory leak problem
- Fixed tethering problem with iOS14 system
- Fixed the problem that port 53 is exposed to the WAN after opening Override DNS Settings for All Clients
- Fixed the problem that the client of the router cannot access the address of the WireGuard server when using WireGuard client
- Fixed the problem that the WireGuard client AllowedIPs parameter does not take effect
- Fixed the problem that Mullvad WireGuard needs to manually modify the MTU to 1380
- Fixed the X1200 dual-module IP exchange problem
- Fixed the problem that some websites cannot be opened after using VPN policy (AR750S, X1200)
- Fixed other known issues

## V3.027 - Oct 16, 2019

- Firmware file: [openwrt-ar750-3.027.bin](https://fw.gl-inet.com/firmware/ar750/v1/openwrt-ar750-3.027.bin)

    MD5: 5585bdce4535714dc55b3d6bae3eb058

**New Features:**

- Added guest wifi
- Added site to site
- Added keeping installed package when upgrade
- Added VPN Policies
- Added Cloud/DDNS
- Added Captive Portal
- Added static IP address binding in LAN IP settings
- Added DHCP address pool
- Added libustream-openssl modem which support download firmware and software package in https

**Fixed:**

- Removed company MAC address detection

---



## V3.010 - Dec 26, 2018

- Firmware file: [gl-ar750-3.010.bin](https://fw.gl-inet.com/firmware/ar750/v1/openwrt-ar750-3.010.bin)

    MD5: 852a34f053999c961815bf43c3e4a84e

**New Features:**

- OpenWrt Updated to version 18.06.
- Adopted new user-interface.
- WireGuard Server/Client pre-installed, supports Azirevpn and Mullvad service providers.
- Support DNS over TLS from Cloudflare.
- Support various 5GHz Wi-Fi speed configurations.
- Added [GL Cloud](../../tutorials/cloud/).
- Added new [DDNS](../../tutorials/ddns/) function.
- Added client management feature which includes QoS, traffic statistics.
- Added firewall settings page which includes port forwards, open port and DMZ.

**Fixed:**

- Improved the stability of wireless connection.
- Removed UPnP server, PPTP and L2TP.

