# Getting Started with VIXMINI

Model: VIXMINI

![router](https://static.gl-inet.com/docs/en/3/setup/vixmini/first_time_setup/router.jpg){class="glboxshadow"}

---

## 1. Power on 

Plug the Micro USB power cable into the power port of the router. Make sure you are using a standard 5V/1A power adapter. Otherwise it may cause malfunction.

![Power on](https://static.gl-inet.com/docs/en/3/setup/vixmini/first_time_setup/power.jpg){class="glboxshadow"}

## 2. Connect 

You can connect to the router via Wi-Fi.

*Note: This step only connects your devices to the local area network (LAN) of the router. You cannot access the Internet currently. In order to connect to the Internet, please finish the setup procedures below and then follow [Internet](../internet) to set up an Internet connection.*

### Connect via Wi-Fi 

Search for the SSID of the router in your device and input the default password: ***goodlife***.

*Note: The SSID was printed on the bottom label of the router with the following format:*

- **VIXMINI-XXX**

*Note: **VIXMINI** has only 1 Ethernet port which works as WAN. You can only connect to it via Wi-Fi when you first set up the router. Once you have connected to it, you can change the WAN port to LAN port in [Internet](../internet#1-cable) so that you can connect to it via LAN.*

## 3. Access the web Admin Panel

Open a web browser (we recommend Chrome, firefox) and visit [http://192.168.8.1](http://192.168.8.1). You will be directed to the initial setup of the web Admin Panel. 

### 1) Language Setting

You need to choose the display language of the Admin Panel. Currently, our routers support **English**, **简体中文**, **繁體中文**, **Deutsch**.

![initial setup](https://static.gl-inet.com/docs/en/3/setup/vixmini/first_time_setup/welcome.jpg){class="glboxshadow"}

*Note: If your browser always redirects to LuCI (http://192.168.8.1/cgi-bin/luci), you can visit: [http://192.168.8.1/index](http://192.168.8.1/index) instead of [http://192.168.8.1](http://192.168.8.1).*

### 2) Admin Password Setting

There is no default password for this Admin Panel. You have to set your own password, which must be at least 5 characters. Then, click `Submit` to proceed.

![password](https://static.gl-inet.com/docs/en/3/setup/vixmini/first_time_setup/password.jpg){class="glboxshadow"}

*Note: This password is for this web Admin Panel and the embedded Linux system. It will not change your Wi-Fi password.*

### 3) Admin Panel

After the initial setup, you will enter the web Admin Panel of the router. It allows you to check the status and manage the settings of the router.

![admin panel](https://static.gl-inet.com/docs/en/3/setup/vixmini/first_time_setup/main_ui.jpg){class="glboxshadow"}
