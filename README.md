# Mozilla-Blocker
### The Great Blocklists to prevent all Mozilla spying and data collecting efforts on their users.

# Userful only in Systemwide Ad-blockers, DNS Sinkholes and for host blocking.

# Direct Links to Mozilla Blocker filters
## For Zen Privacy Guard,Adguard Home and Pi-hole - https://raw.githubusercontent.com/gitfilts/Mozilla-Blocker/refs/heads/main/MozillaBlockerAdblock.txt

### For Windows host and Android Adaway - https://raw.githubusercontent.com/gitfilts/Mozilla-Blocker/refs/heads/main/MozillaBlockerHost.txt

### Recommended Systemwide Adblocker - https://github.com/anfragment/zen
### Recommended DNS Network-wide Adblocker - https://github.com/AdguardTeam/AdGuardHome

### This filter is also useful in Adguard for Windows and Android but you must enable DNS Protection and add the filter as a DNS Filter. If you already use Adguard home or Pi-hole and add the list there, then Adguard for windows app won't provide extra advantage.

### Just like how uBlock Origin and uMatrix/nuMatrix can't detect and block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites in firefox and modern firefox forks due to some kind of policy forced onto extension makers by Mozilla. Adguard for windows and android also doesn't detect https google tracking request and scripts on mozilla websites like Mozilla Add-ons while using any broswers, it can only block dns requests of those google requests.
### So I don't really recommend relying on Adguard systemwide adblocker for firefox or any of the firefox fork users, otherwise Adguard is very good for other browser users.
### Among all the firfox forks, only old forks like Palemoon and Basilisk doesn't have this sort of forced privacy violating policy enforced on them by Mozilla.
### uBlock Origin Legacy(ublock fork) and nuMatrix(uMtrix fork) can block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites on Palemoon and Basilisk. Blocking these google trackers with a dns adblocker like adguard home and pi-hole should be enough to prevent tracking, but those can't prevent those scripts from running on mozilla websites in firefox or all standard firefox forked browser.
