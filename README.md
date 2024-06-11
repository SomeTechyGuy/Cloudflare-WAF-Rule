# Cloudflare-WAF-Rule
A Powerful Cloudflare WAF Anti DDoS rule I made for preventing bots, VPNs/Proxies, Old browsers, and Cloud IPs from accessing your website.

## WAF Rule Details

The included items in my Cloudflare WAF rule is:

- Any bot detected by Cloudflare
- Chrome version 30-109
- Many cloud ASNs

### Rule Conditions
- Make sure to set the action to block before deploying

```plaintext
(cf.client.bot) or 
(http.user_agent eq "vercel-fetch") or
(ip.src eq 209.251.16.230) or
(ip.geoip.asnum in {16509 11878 14061 46261 46664 207990 611 9009 132203 132153 136907 51852 396982 27176 14618 212238 24940 50613 12876 63199 45090 63949 16276 18779 203999 55286 21769 60781 64267 210558 45102 3462 8075 4766 31898 8151 4314 3223 2514 63473 398101 26496 397336 46562 39690 62567 135340 200130 201229 202018 202109 205301 393406 394362 2 398712 8560 398324 3352 8100 397373 13768 202425 137409 400536}) or 
(http.user_agent contains "Chrome/7") or 
(http.user_agent contains "Chrome/5") or 
(http.user_agent contains "Chrome/8") or 
(http.user_agent contains "Chrome/6") or 
(http.user_agent contains "Chrome/9") or
(http.user_agent contains "Chrome/10")
or
(http.user_agent contains "Chrome/3")
or
(http.user_agent contains "Chrome/4")
