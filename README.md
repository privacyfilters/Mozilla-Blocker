# Mozilla-Blocker
#### The Great Blocklists to prevent all Mozilla spying and data collecting efforts on their users.

# Useful only with Systemwide Ad-blockers, DNS Sinkholes and host blocking.

## Filters which allows firefox forks to install and update add-ons from mozilla extension store
Adguard Home and Zen Privacy Guard - https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/adblock_dns.txt

Windows/Linux host and Android Adaway - https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/hosts.txt

## No Mozilla Version - Everything is blanket blocked from Mozilla, including Add-ons.
Adguard Home and Zen privacy Guard - https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/adblock_dns_nomozilla

Windows/Linux host and Android Adaway - https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/hosts_nomozilla

## Recommended Methods to Block Mozilla
DNS Network-wide Adblocker- Adguard Home - https://github.com/AdguardTeam/AdGuardHome

Systemwide Adblocker - Zen Privay Guard - https://github.com/anfragment/zen

These filters works perfectly on Adguard Home.
Zen privacy guard is still early on development so it is unstable when enforcing the filters.
I don't know if these rules will work correctly on pi-hole as I use Adguard Home and they works prefectly fine there. 

## Mozilla also uses Google trackers on their sites which they don't allow adblockers to detect and report to the user
UBlock Origin and uMatrix/nuMatrix can't detect and block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites in firefox and modern firefox forks due to some kind of policy forced onto extension makers by Mozilla. Adguard for windows and android also doesn't detect https google tracking request and scripts on mozilla websites like Mozilla Add-ons while using any broswers, even in chrome.

So I don't really recommend relying on Adguard systemwide adblocker for firefox or any of the standard firefox fork users, otherwise Adguard is very good for other browser users. In app DNS filterer is still good and will block every trackers without mozilla interventions.

Among all the firfox forks, only unique forks like Palemoon and Basilisk doesn't have this sort of forced privacy violating policy enforced on them by Mozilla.
uBlock Origin Legacy(ublock fork) and nuMatrix(uMtrix fork) can block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites on Palemoon and Basilisk. Blocking these google trackers with a dns adblocker like adguard home and pi-hole should be enough to prevent tracking, but those can't prevent those scripts from running on mozilla websites in firefox or all standard firefox forked browser.
