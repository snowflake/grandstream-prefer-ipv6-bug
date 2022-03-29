# Grandstream Prefer IPv6 Bug - Phone will not use an IPv4 SIP Account

Research to find out why my [Grandstream](https://www.grandstream.com)
phone does not use an IPv4 SIP account when Prefer IPv6 is enabled.

For full details, please vist our [wiki](https://github.com/snowflake/grandstream-prefer-ipv6-bug/wiki) on Github.

I have a Grandstream GRP2612 VOIP phone which I have owned since 2019.  It works well and I have had no real problems with it until now.

I have two SIP accounts with different providers.

One provider supplies service over IPv4 only, and the
other provider supports both IPv4 and IPv6 service.

In March 2022, I decided to test whether the phone works over IPv6. My ISP
does not provide IPv6 access at the moment, so I set up an IPv6 tunnel with
[Hurricane Electric](https://he.net)

On the phones' System settings under Network, I set the Internet Protcol to
Prefer IPv6 and saved the setting.

I then rebooted the phone.

It is very important that the phone be rebooted, otherwise the new setting
does not take affect. The phone does not warn you about this. It only warns you if you use the phone's local web page to change the settings.

When the phone had finished rebooting and after waiting a minute for the
accounts to register, I found that only the IPv4+IPv6 account had 
registered.

This was annoying to say the least.

I captured the packets to and from the phone using such tools as tcpdump and Wireshark. I found that there were some interesting anomalies.

For full details, please vist our [wiki](https://github.com/snowflake/grandstream-prefer-ipv6-bug/wiki) on Github.
