# Pi-hole lists (rebuilt 2026-11-15)

Plain-domain lists, deduplicated across files in the order below (each domain appears once).
Import each as an adlist; `allow.txt` is the allowlist (exact domains).

| File | Upstream (HaGeZi base: https://raw.githubusercontent.com/hagezi/dns-blocklists/main/wildcard/) |
|---|---|
| hagezi-pro.txt | pro-onlydomains.txt |
| hagezi-social.txt | social-onlydomains.txt (Facebook, Instagram, TikTok, X, Snapchat; not WhatsApp) |
| hagezi-tiktok-extended.txt | native.tiktok.extended-onlydomains.txt |
| hagezi-native-devices.txt | native.{samsung,lgwebos,xiaomi,huawei,oppo-realme,vivo,roku}-onlydomains.txt |
| hagezi-doh-vpn-bypass.txt | doh-vpn-proxy-bypass-onlydomains.txt (stops DoH/VPN bypassing Pi-hole) |
| hagezi-dyndns.txt | dyndns-onlydomains.txt (ennor.ddns.net is in allow.txt) |
| hagezi-fake.txt | fake-onlydomains.txt (scam/fake shops; replaces add-spam) |
| w3kbl.txt | https://v.firebog.net/hosts/static/w3kbl.txt |
| kad-hosts.txt | https://raw.githubusercontent.com/FiltersHeroes/KADhosts/master/KADhosts.txt |
| cert-polska.txt | https://hole.cert.pl/domains/v2/domains_hosts.txt |
| hagezi-tif-medium.txt | tif.medium-onlydomains.txt |
| oisd-nsfw.txt | https://nsfw.oisd.nl/domainswild2 |
| allow.txt | anudeepND commonly-whitelisted domains + ennor.ddns.net (t.co/twimg.com removed: social is blocked on purpose) |

Pi-hole matches exact domains only. Full TIF (1.45M) swapped for tif.medium.
Skipped native lists that break things: amazon, apple, winoffice.
