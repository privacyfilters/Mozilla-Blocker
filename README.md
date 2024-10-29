# Mozilla-Blocker
### The Great Blocklists to prevent all Mozilla spying and data collecting efforts on their users.

# Userful only in Systemwide Ad-blockers, DNS Sinkholes and for host blocking.

## Direct Links to Mozilla Blocker filters
For Zen Privacy Guard, Adguard Home and Pi-hole - https://raw.githubusercontent.com/gitfilts/Mozilla-Blocker/refs/heads/main/MozillaBlockerAdblock.txt

For Windows host and Android Adaway - https://raw.githubusercontent.com/gitfilts/Mozilla-Blocker/refs/heads/main/MozillaBlockerHost.txt

## Recommended Methods to Block Mozilla
Systemwide Adblocker - Zen Privay Guard - https://github.com/anfragment/zen
DNS Network-wide Adblocker- Adguard Home - https://github.com/AdguardTeam/AdGuardHome

## Mozilla also uses Google trackers on their sites which they don't allow adblockers to detect
UBlock Origin and uMatrix/nuMatrix can't detect and block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites in firefox and modern firefox forks due to some kind of policy forced onto extension makers by Mozilla. Adguard for windows and android also doesn't detect https google tracking request and scripts on mozilla websites like Mozilla Add-ons while using any broswers, even in chrome.

So I don't really recommend relying on Adguard systemwide adblocker for firefox or any of the standard firefox fork users, otherwise Adguard is very good for other browser users. In app DNS filterer is still good and will block every trackers without mozilla interventions.

Among all the firfox forks, only unique forks like Palemoon and Basilisk doesn't have this sort of forced privacy violating policy enforced on them by Mozilla.
uBlock Origin Legacy(ublock fork) and nuMatrix(uMtrix fork) can block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites on Palemoon and Basilisk. Blocking these google trackers with a dns adblocker like adguard home and pi-hole should be enough to prevent tracking, but those can't prevent those scripts from running on mozilla websites in firefox or all standard firefox forked browser.
