# grandstream-prefer-ipv6-bug

Research to find out why my Grandstream phone does not use an IPv4 SIP account when Prefer IPv6 is enabled.

I have a Grandstream GRP2612 VOIP phone which I have owned since 2019.  It works well and I have had no real problems with it.

I have two SIP accounts with different providers.

One provider supplies service over IPv4 only, and the
other provider supports both IPv4 and IPv6 service.

In March 2022, I decided to test whether the phone works over IPv6. My ISP
does not provide IPv6 access at the moment, so I set up an IPv6 tunnel with
[Hurricane Electric](https://he.net)
