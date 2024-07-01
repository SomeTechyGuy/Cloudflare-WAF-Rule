# Cloudflare-WAF-Rule
A Powerful Cloudflare WAF Anti DDoS rule I made that has even been tested by a real DDoS service for preventing bots, VPNs/Proxies, Old browsers, and Cloud IPs from accessing your website.

## WAF Rule Details

The included items in my Cloudflare WAF rule is:

- Any bot detected by Cloudflare
- Chrome version 30-109
- Many cloud ASNs
- Firefox 30-79

### How to add the rule
- Before making the rule please make sure to turn off bot fight mode if it's on.
- Copy [this rule](https://cstuff.cz/Cloudflare-WAF-rule.txt) or the one in [Mirror 1](https://raw.githubusercontent.com/SomeTechyGuy/Cloudflare-WAF-Rule/main/AntiDDos.txt) or in [Mirror 2](https://gitlab.com/cjhar1224/My-website/-/raw/main/public/Cloudflare-WAF-rule.txt) and then paste it into the Cloudflare WAF rule you made.
- Now set the action to block, click deploy, and then most DDoSes, users with proxies or VPNs, bots, and cloud providers should be blocked.
