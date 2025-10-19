# Mozilla Blocker - Block all Mozilla/Firefox Spying
#### The Great Blocklists to prevent all Mozilla spying and data collecting efforts on their users.
### [Codeberg](https://github.com/privacyfilters/Mozilla-Blocker) is the home of Mozilla Blocker. Its mirrored at github for backup and availability. Use only one filter source.
### Available on both [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker) and [Github](https://github.com/privacyfilters/Mozilla-Blocker)(mirror).
# Useful only with Systemwide Ad-blockers, DNS Sinkholes and host blocking. 

## Regualr Version : Filters which allows firefox forks to install and update add-ons from mozilla extension store
#### Adguard Home and Zen Adblocker - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/adblock_dns.txt) - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/adblock_dns.txt)

#### Windows/Linux host, Opensnitch and Android Adaway - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts) - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/hosts)

## No Mozilla Version: Everything is blanket blocked from Mozilla, including Add-ons. Not recommended for Regular users
#### Adguard Home and Zen Adblocker - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/adblock_dns_nomozilla.txt) - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/adblock_dns_nomozilla.txt)

#### Windows/Linux host, Opensnitch and Android Adaway - [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts_nomozilla) - [Github](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/refs/heads/main/hosts_nomozilla)

## Recommended Methods to Block Mozilla
1. DNS Network-wide Adblocker- Adguard Home (stable)(foss)(dns) - https://github.com/AdguardTeam/AdGuardHome
2. Systemwide Adblocker for Widnows/Linux- Zen Privay Guard (semi-stable)(foss)(adblock)- https://github.com/anfragment/zen
3. SwitchHosts for Windows (unstable)(foss)(hosts) - https://github.com/oldj/SwitchHosts
4. hosty for Linux (stable)(foss)(hosts) - https://github.com/astrovm/hosty
5. Opensnitch firewall for Linux (foss)(hosts) - https://github.com/evilsocket/opensnitch
6. personelDNSfilter for Android (stable)(no-root)(foss)(hosts)(dns) - https://github.com/IngoZenz/personaldnsfilter
7. Netguard firewall for Android (stable)(no-root)(foss)(hosts) - https://github.com/M66B/NetGuard
8. Adaway for Android (root)(no-root)(stable)(foss)(hosts) - https://github.com/AdAway/AdAway
9. Adguard for Android as Dns protection (no-root)(stable)(non-foss)(paid-app)(dns) - https://adguard.com/en/adguard-android/overview.html

The adblock filter format works perfectly on Adguard Home.
Zen adblocker is still early on development so it is unstable when enforcing the filters.
Host rules will work with anything just as a host file for any platform and with blockers that supports host format.
I don't know if the adblock_dns formate of rules will work correctly on pi-hole as I only used Adguard Home and they works fine there. 

## Alternative Sources of Mozilla Blocker
## Codeberg Version - https://codeberg.org/privacyfilters/Mozilla-Blocker <br>Github Version - https://github.com/privacyfilters/Mozilla-Blocker

## Mozilla also uses Google trackers on their sites which they don't allow adblockers to detect and report to the user
UBlock Origin and uMatrix/nuMatrix can't detect and block google tracking scripts from google-analytics.com and googletagmanager.com on the mozilla site - "Mozilla-Addons", on firefox and modern firefox forks due to policy forced onto extension makers by Mozilla, probably with the excuse of security. Adguard for windows and android also doesn't detect https google tracking request and scripts on mozilla websites like Mozilla Add-ons while using any broswers, even on chrome.

So I don't really recommend relying on Adguard systemwide adblocker for firefox or any of the standard firefox fork users, otherwise Adguard is good for other browser users. In app DNS filterer is still good and will block every trackers without mozilla policy interventions.

Among all the firfox forks, only unique forks like Palemoon and Basilisk doesn't have this sort of forced privacy violating policy enforced on them by Mozilla. But these browsers suffers from performance and stabitlity issues frequently. So blocking Mozilla on system/dns level and using modern firefox forks like librewolf, floorp, zen etc would be more suited to have a regular comfortable usage experience.

uBlock Origin Legacy(ublock fork) and nuMatrix(uMtrix fork) can block google tracking scripts from google-analytics.com and googletagmanager.com on mozilla websites on Palemoon and Basilisk. Blocking these google trackers with a dns adblocker like adguard home and pi-hole should be enough to prevent tracking, but those can't prevent those scripts from running on mozilla websites in firefox or all standard firefox forked browser. For more security and privacy aware people, this can be an issue where regular users would be just fine blocking mozilla systemwide with dns/host blocking.

# Userful Infos and Resources for firefox and firefox based browsers

## 1. [Hagezi Dns-blocklists](https://github.com/hagezi/dns-blocklists) - Currently the best maintained collection of filters for privacy, security and blocking ads and trackers. Must have for any blocking system.
I use several Hagezi filters on my AdguardHome server, Adguard for android, Adaway, in all adblockers on the browsers I use. For most people, the Pro and  Threat Intelligence Feeds along will cover all your ads, tracking and security concern. You can use the Ultimate filter if you don't mind ublocking specific domains of the services you use which are blocked.

## 3. [yokoffing filterlists](https://github.com/yokoffing/filterlists) - Recommened for most general Users. A balanced sets of adblocking and privacy filteres for adblockers are Ublock Origin, Adguard and Brave browser.
Just configure your adblocker like ublock origin and adguard for any browsers and enjoy a cleaner, faster internet with most of tracking from websites blocked, without sacrificing any browser performance which can be caused by some privacy enhacing methods.

## 3. [Phoenix](https://codeberg.org/celenity/Phoenix) - Phoenix is a suite of configurations & advanced modifications for Mozilla Firefox. Only for people who wants the maximum privacy. For performance, instead of this, use a good firefox fork by manually changing browser settingsand ublock origin filters.
This is mostly automated for linux distros. You just need to install it once using your packag manager. You can also install firefox official browser using package manager of your linux distro, you don't need to access to mozilla servers. For windows users, you need access to mozilla ftp to download the installer, which I kept blocked because mozilla also use their ftp urls for tracing calls! You should just use a firefox fork if you won't use Phoenix.

## 4. [BadBlock](https://codeberg.org/celenity/BadBlock) - According to celenity, both Phoenix and BadBlock's author - "BadBlock is a collection of comprehensive blocklists that I personally maintain covering a variety of different services, applications, & platforms with the goal of blocking... well, as the name suggests, stuff that is bad™".
A good collection of privacy focused filter lists, which are not covered by yokoffing. You can use them to enhance your privacy and security if you are interested.
## 5. [LibreWolf](https://librewolf.net/) - A custom version of Firefox, focused on privacy, security and freedom.
Probably the most mozilla tracking free firefox fork out of the box. It still calls some mozilla connections, which are minimal. For privacy conscious people, I will mostly suggest to use either firefox official+Phoenix or libreewolf+Ublock origin with yokoffing filters. Phoenix for librewolf would have been wonderful, I do hope someday [celenity](https://codeberg.org/celenity) will start supporting librewolf browser alongside with firefox.

## 6. [Zen Browser](https://zen-browser.app/) - Trending firefox fork with tones of features and sidetab by default. Currently one of two most good looking and performant firefox forks. Not privacy focused.
Makes tones of home calls to zen browser domain. you should just block zen-broser.app domain, and install the borwser with a package manager of your linux distro, UnigetUi for microsoft widnows(winget,chocoletey) or just directly download the installer from their [github releases](https://github.com/zen-browser/desktop/releases).

## 7. [Floorp Browser](https://floorp.app/) - A very good looking, customizable and performant firefox fork. Used to be called vivaldi of firefox. Not Privacy focused.
It is very fast, it was a delight to use as my default browser before I switched to Brave browser. It has many customization options but not as many as zen browser. It calls home less than zen browser, which is a good thing. But it does call home for occasional updates. You can just block floorp domains like floorp.app and others and use package managers to install and update the browser, or directly download the installer from their [github releases](https://github.com/Floorp-Projects/Floorp/releases).