# Self-Hosted Network Docs Site

> A lightweight, offline compatible docs site.

Welcome, everyone!

# What is this network?

This self-hosted network is a unified collection of free tools and services that provide a high degree of control, security, and privacy over your digital infrastructure. Our set-up includes a combination of ZeroTier and Tailscale – both of which are top-tier services that enable the creation of software-defined networks.

ZeroTier is a smart Ethernet switch for planet Earth. It connects devices, cloud VMs, and apps anywhere as though they were all on the same local network. With ZeroTier, we're able to provide end-to-end encrypted connections with mobility, elasticity, and ease-of-use, without the hassle of traditional VPN configurations.

Tailscale, on the other hand, is built on top of the WireGuard® protocol, delivering an incredibly secure and lean VPN experience. It builds mesh networks of your devices to connect them together securely and privately. Tailscale simplifies the process of creating and maintaining a VPN and works seamlessly across your phones, tablets, computers, and servers - even when they are behind NATs or changing networks.

By leveraging the strengths of both ZeroTier and Tailscale, our self-hosted network creates a secure and seamless network that stretches across all your devices, regardless of their location. Both services are known for their ease of use and minimal configuration, making them accessible for everyone, from IT professionals to those just starting with network management.

This hybrid approach enables us to:

- Connect a variety of devices with different operating systems.
- Enable secure access to internal services without exposing them to the public internet.
- Maintain complete control over our networking stack, avoiding reliance on third-party central servers for network management and control.
- Create customized networks that match our precise use cases and requirements.

Our self-hosted network is designed to be scalable, flexible, and resilient, capable of supporting a range of applications from secure file sharing and collaboration to hosting personal websites and services.

Through the detailed guides in this documentation site, you'll learn how to set up, manage, and utilize this network to bring efficiency and enhanced privacy to your operations.

# Hosts File

The hosts file is a simple text file used by an operating system to map hostnames to IP addresses. Whenever you type a domain name into your web browser, your system checks the hosts file to see if there's a corresponding IP address specified, before reaching out to a DNS server. Editing the hosts file can be useful for testing a website without changing DNS settings, blocking access to certain domains, or simplifying access to devices within your network by assigning familiar names instead of remembering IPs.

## How to change on Windows

1. Open Notepad with Administrator privileges by right-clicking on the app in the Start Menu and choosing 'Run as administrator'.
2. Go to File > Open and navigate to `C:\Windows\System32\drivers\etc\hosts`.
3. Make the necessary changes to the file. For example, to map `192.168.1.5` to `myserver.local`, simply add the line `192.168.1.5 myserver.local` at the end of the file.
4. Save your changes and close Notepad. The changes should take effect immediately without the need to reboot.

## How to change on Linux

1. Open a terminal window.
2. Use a text editor with sudo privileges to edit the hosts file by running `sudo nano /etc/hosts` (you can replace `nano` with your preferred text editor).
3. Add the mappings that you need following the same format as in Windows, such as `192.168.1.5 myserver.local` at the end of the file.
4. Save the file and exit the text editor. For nano, you would press `Ctrl+O` to write out the changes, hit `Enter` to confirm, and then `Ctrl+X` to exit.
5. After you exit the editor, the new mappings are available for use.

# Mobile Device Configuration (ZeroTier)

Configuring ZeroTier on mobile devices enables you to securely connect your smartphones and tablets to your self-hosted network.

## For iOS and Android:

1. Download and install the ZeroTier One app from the App Store or Google Play Store.
2. Open the app and create an account or log in if you already have one.
3. Join a network by tapping the '+' button and entering the Network ID of your ZeroTier network. This ID can typically be obtained from the ZeroTier Central web interface.
4. Once the network is joined, the ZeroTier service will request authorization for your new device. This usually needs to be done from the ZeroTier Central web panel by an authorized network administrator.
5. After your device is authorized, it will automatically receive an IP address from the ZeroTier network and establish secure, encrypted connections to other devices on the network.

For further details and troubleshooting, please refer to the appropriate sections within this documentation or visit the official ZeroTier Knowledge Base.

