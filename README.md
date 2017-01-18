# steamcache
Cache steam games using dnsmasq and nginx

***Introduction***

These config files configure nginx and dnsmaq to be a fairly quick caching proxy to make downloading games multiple times less WAN intensive

***Usage***

0. Install nginx and dnsmasq
1. Place the nginx.conf in /etc/nginx/
2. Place the nginx-steam-cache.conf in /etc/ngnix/nginx.d/
3. Place dnsmasq-steam-cache.conf in /etc/dnsmasq.d/
4. Restart both processes

***Is it working?***

Use the following command to see if subsequent game downloads being sourced from cache (HIT):
> tailf /var/log/nging/steamcontent.access.log
