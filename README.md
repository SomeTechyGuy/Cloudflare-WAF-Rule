# Cloudflare-WAF-Rule
A Powerful Cloudflare WAF Anti DDoS rule I made for preventing bots, VPNs/Proxies, Old browsers, and Cloud IPs from accessing your website.

## WAF Rule Details

The included items in my Cloudflare WAF rule is:

- Any bot detected by Cloudflare
- Chrome version 30-109
- Many cloud ASNs
- Firefox 30-79

### How to add the rule
- Before deployment please make sure to set the action to block.
- Copy the [rule](https://cstuff.cz/Cloudflare-WAF-rule.txt) and then paste it into the Cloudflare WAF rule.
- Click deploy and then most DDoSes, users with proxies or VPNs, bots, and cloud providers should be blocked.
