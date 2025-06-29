
In these examples, 1.2.3.4 represents the [LAN side IP address](https://www.computerworld.com/article/2474776/network-security/find-the-ip-address-of-your-home-router.html) of the router.

In June 2020 we learned that 79 different Netgear devices [shared the same flaw](https://blog.grimm-co.com/2020/06/soho-device-exploitation.html). A bad guy can learn the exact model and firmware of a Netgear router using a URL like
   [https://1.2.3.4/currentsetting.htm](https://1.2.3.4/currentsetting.htm)
and customize an exploit specifically for that router. If you have a Netgear router, try this URL. If it returns information about your router, look for the most recent firmware. Hopefully, it will have been released after June 2020. At the time when the flaw was made public (June 15, 2020) Netgear had done nothing regarding a fix.

In October 2019 we learned of [10 D-Link routers](https://kb.cert.org/vuls/id/766427/) with critical flaws that will not be fixed. If you have any of these D-Link routers, don't bother testing, just get a new router: DIR-655, DIR-866L, DIR-652, DHP-1565, DIR-855L, DAP-1533, DIR-862L, DIR-615, DIR-835 and the DIR-825. For confirmation, CERT has a [Proof of Concept](https://kb.cert.org/artifacts/cve-2019-16920.html) web page that will disconnect a vulnerable D-Link router from the Internet for a minute.

In January 2019 we learned of two [information disclosure bugs](https://badpackets.net/over-9000-cisco-rv320-rv325-routers-vulnerable-to-cve-2019-1653/) in some Cisco routers. More details are on the Bugs page. If the URL below shows details about your Cisco router, that is bad. A public/WAN side version of this is auto-generated on the [Shodan](https://routersecurity.org/shodan.php) page.
   [https://1.2.3.4/cgi-in/config.exp](https://1.2.3.4/cgi-in/config.exp)
   [https://1.2.3.4/cgi-bin/export_debug_msg.exp](https://1.2.3.4/cgi-bin/export%5C%5C_debug%5C%5C_msg.exp)

As per Scott Helme's 2014 [description of his BrightBox router](https://scotthelme.co.uk/ee-brightbox-router-hacked/), try the URL below, where 1.2.3.4 is the IP address of your router. A good result returns nothing but an error message. Here is a [sample](https://scotthelme.co.uk/wp-content/uploads/2014/01/cgi-status-js.png) of a bad result.
   [https://1.2.3.4/cgi/](https://1.2.3.4/cgi/) cgi_status.js

In December 2016, Pedro Ribeiro reported on [flaws in the Netgear WNR2000](https://seclists.org/fulldisclosure/2016/Dec/72) router. If you own a Netgear router, it can't hurt to check for information leakage with the URL below. It may leak the device serial number.
   [https://1.2.3.4/](https://1.2.3.4/) BRS_netgear_success.html

Many Netgear routers had a security flaw in December 2016 (see [here](https://www.computerworld.com/article/3151097/security/updates-and-more-on-the-netgear-router-vulnerability.html)
and [here](https://www.computerworld.com/article/3148680/networking/easily-exploited-netgear-router-flaw-discovered.html) for more). The command below tests a Netgear router. If this results in a web page with the word "Vulnerable", then the [router is vulnerable](https://www.heise.de/security/meldung/Netgear-Luecke-dramatischer-als-angenommen-erste-Sicherheits-Updates-3569299.html). Netgear has issued fixes for all vulnerable routers.
  [https://www.routerlogin.net](https://www.routerlogin.net/) /cgi-bin/;echo$IFS'Vulnerable'

This issue with port 32764 is explained above in the [TCP Ports to Test](https://routersecurity.org/testrouter.php#TCPport32764) section.
   [https://1.2.3.4:32764](https://1.2.3.4:32764/)

In September 2017, security firm Embedi found port 19541 [open on many D-Link routers](https://embedi.com/blog/enlarge-your-botnet-top-d-link-routers-dir8xx-d-link-routers-cruisin-bruisin). It responds to commands such as one to reboot the router. They did not find any way to close the port. The default IP address is 192.168.0.1 but the router may also respond to dlinkrouter.local.
   [https://1.2.3.4:19541](https://1.2.3.4:19541/)
