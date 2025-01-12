# Mozilla Blocker - The Great Filters to Block All Mozilla Spying
#### The Great Blocklists to prevent all Mozilla spying and data collecting efforts on their users.
### Available on [Github](https://github.com/privacyfilters/Mozilla-Blocker) and [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker).
# Useful only with Systemwide Ad-blockers, DNS Sinkholes and host blocking.

## Filters which allows firefox forks to install and update add-ons from mozilla extension store
#### Adguard Home and Zen Adblocker - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/adblock_dns.txt) - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/adblock_dns.txt)

#### Windows/Linux host, Opensnitch and Android Adaway - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/hosts) - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts)

## No Mozilla Version - Everything is blanket blocked from Mozilla, including Add-ons
#### Adguard Home and Zen Adblocker - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/adblock_dns_nomozilla.txt) - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/adblock_dns_nomozilla.txt)

#### Windows/Linux host, Opensnitch and Android Adaway - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/hosts_nomozilla) - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts_nomozilla)

## Recommended Methods to Block Mozilla
1. DNS Network-wide Adblocker- Adguard Home (stable)(foss)(dns) - https://github.com/AdguardTeam/AdGuardHome
2. Systemwide Adblocker for Widnows/Linux- Zen Privay Guard (semi-stable)(foss)(adblock)- https://github.com/anfragment/zen
3. SwitchHosts for Windows (unstable)(foss)(hosts) - https://github.com/oldj/SwitchHosts
4. hosty for Linux (stable)(foss)(hosts) - https://github.com/astrovm/hosty
5. Opensnitch firewall for Linux (foss)(hosts) - https://github.com/evilsocket/opensnitch
6. personelDNSfilter for Android (stable)(no-root)(foss)(hosts)(dns) - https://github.com/IngoZenz/personaldnsfilter
7. Netguard firewall for Android (stable)(no-root)(foss)(hosts) - https://github.com/M66B/NetGuard
8. Adaway for Android (root)(stable)(foss)(hosts) - https://github.com/AdAway/AdAway
9. Adguard for Android as Dns protection (no-root)(stable)(non-foss)(paid-app)(dns) - https://adguard.com/en/adguard-android/overview.html

The adblock filter format works perfectly on Adguard Home.
Zen privacy guard is still early on development so it is unstable when enforcing the filters.
Host rules will work with anything just as a host file for any platform and with blockers that supports host format.
I don't know if the adblock_dns formate of rules will work correctly on pi-hole as I only used Adguard Home and they works fine there. 

## Alternative Sources of Mozilla Blocker
## Codeberg Version - https://codeberg.org/privacyfilters/Mozilla-Blocker <br>Github Version - https://github.com/privacyfilters/Mozilla-Blocker

## Mozilla also uses Google trackers on their sites which they don't allow adblockers to detect and report to the user
UBlock Origin and uMatrix/nuMatrix can't detect and block google tracking scripts from google-analytics.com and googletagmanager.com on the mozilla site - "Mozilla-Addons", on firefox and modern firefox forks due to policy forced onto extension makers by Mozilla, probably with the excuse of security. Adguard for windows and android also doesn't detect https google tracking request and scripts on mozilla websites like Mozilla Add-ons while using any broswers, even on chrome.

So I don't really recommend relying on Adguard systemwide adblocker for firefox or any of the standard firefox fork users, otherwise Adguard is good for other browser users. In app DNS filterer is still good and will block every trackers without mozilla policy interventions.

Among all the firfox forks, only unique forks like Palemoon and Basilisk doesn't have this sort of forced privacy violating policy enforced on them by Mozilla. But these browsers suffers from performance and stabitlity issues frequently. So blocking Mozilla on system/dns level and using modern firefox forks like librewolf, floorp, zen etc would be more suited to have a regular comfortable usage experience.

uBlock Origin Legacy(ublock fork) and nuMatrix(uMtrix fork) can block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites on Palemoon and Basilisk. Blocking these google trackers with a dns adblocker like adguard home and pi-hole should be enough to prevent tracking, but those can't prevent those scripts from running on mozilla websites in firefox or all standard firefox forked browser. For more security and privacy aware people, this can be an issue where regular users would be just fine blocking mozilla systemwide with dns/host blocking.


