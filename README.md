# Mozilla Blocker: Block All Mozilla/Firefox Spying

**Blocklists to stop Mozilla's tracking and data collection on their users.**

Mozilla Blocker is a set of filters that block everything from Mozilla including their telemetry, tracking, analytics and other "phone home" connections made by Firefox and Firefox-based browsers.

There are two versions, depending on whether you still want to install add-ons:

* 🟢 **[Regular](#filter-regular)**: blocks everything from Mozilla, but still lets Firefox forks install and update add-ons from the Mozilla extension store
* 🔴 **[No Mozilla](#filter-no-mozilla)**: blanket blocks everything from Mozilla, add-ons included. Not recommended for regular users

---

## 📍 Project Home

**Codeberg is the primary home of Mozilla Blocker.**

* **[Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker)**: primary repository
* **[GitHub](https://github.com/privacyfilters/Mozilla-Blocker)**: mirror, kept for backup and availability

> **Please use only one copy of each filter.**
> All sources have the same lists. Using more than one doesn't give you extra protection, it just creates duplicate rules.

> **About jsDelivr:** it caches files, so after an update the CDN links can be several hours behind Codeberg and GitHub. If you need the latest version right away, use Codeberg or GitHub.

---

## ⚠️ Before You Use It

These filters only make sense with **system-wide ad-blockers, DNS sinkholes, and hosts-based blocking**. Browser extensions can't do the job here, since the point is to stop Mozilla connections before they leave your network or device.

---

# 📥 Filter Lists

<a id="filter-regular"></a>

## 🟢 Regular Version

Allows Firefox forks to install and update add-ons from the Mozilla extension store.

| Format | Works with | Codeberg | GitHub | CdnjsDelivr |
| ------ | ---------- | -------- | ------ | -------- |
| **Adblock / DNS** | AdGuard Home, Adblock-Fast, pfSense + pfBlockerNG, Zen Adblocker | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/adblock_dns.txt) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/adblock_dns.txt) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/adblock_dns.txt) |
| **Domains** | Pi-hole, OPNsense, Adblock-lean, personalDNSfilter (raw domains and subdomains) | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/domains.txt) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/domains.txt) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/domains.txt) |
| **DNSMasq** | DNSMasq, Adblock-lean | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/dnsmasq.txt) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/dnsmasq.txt) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/dnsmasq.txt) |
| **Hosts** | Windows/Linux hosts file, OpenSnitch, AdAway | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/hosts) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/hosts) |
| **Hosts-Clean** | Adblock-lean. Identical to Hosts, just with a different name (use it if `hosts` causes an error) | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts-clean) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/hosts-clean) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/hosts-clean) |

### ✅ Whitelist

For tools where you have to allow domains manually (like Adblock-lean, and likely other tools using the plain Domains format such as Pi-hole and OPNsense), use this list. It contains the domains the Regular version keeps unblocked: the add-on install/update endpoints and the Thunderbird/Betterbird email account autoconfig. The file is generated from the same allow categories as the filter lists above, so any future whitelist addition is picked up automatically:

* [Codeberg](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/whitelist_domains.txt)
* [GitHub](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/whitelist_domains.txt)
* [CdnjsDelivr](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/whitelist_domains.txt)

---

<a id="filter-no-mozilla"></a>

## 🔴 No Mozilla Version

Everything from Mozilla is blanket blocked, **including add-ons**. Not recommended for regular users.

| Format | Works with | Codeberg | GitHub | CdnjsDelivr |
| ------ | ---------- | -------- | ------ | -------- |
| **Adblock / DNS** | AdGuard Home, Adblock-Fast, pfSense + pfBlockerNG, Zen Adblocker | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/adblock_dns_nomozilla.txt) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/adblock_dns_nomozilla.txt) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/adblock_dns_nomozilla.txt) |
| **Domains** | Pi-hole, OPNsense, Adblock-lean, personalDNSfilter (raw domains and subdomains) | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/domains_nomozilla.txt) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/domains_nomozilla.txt) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/domains_nomozilla.txt) |
| **DNSMasq** | DNSMasq, Adblock-lean | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/dnsmasq_nomozilla.txt) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/dnsmasq_nomozilla.txt) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/dnsmasq_nomozilla.txt) |
| **Hosts** | Pi-hole, Windows/Linux hosts file, OpenSnitch, AdAway | [Link](https://codeberg.org/privacyfilters/Mozilla-Blocker/raw/branch/main/hosts_nomozilla) | [Link](https://raw.githubusercontent.com/privacyfilters/Mozilla-Blocker/main/hosts_nomozilla) | [Link](https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/hosts_nomozilla) |

---

# 🛡️ Recommended Blocking Methods

## 🌐 Network-wide (most recommended)

| Tool | Type | Format | FOSS | Notes |
| ---- | ---- | ------ | :--: | ----- |
| **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)** | DNS network-wide blocker | Adblock / DNS | ✅ | Stable. Windows, Linux, macOS, OpenWrt |
| **[Pi-hole](https://pi-hole.net/)** | DNS network-wide blocker | Domains | ✅ | Stable. Hosts also works. Unsure about the `$important` rules in Adblock / DNS |
| **[Adblock-lean](https://github.com/lynxthecat/adblock-lean)** | Router blocker (OpenWrt only) | Domains, DNSMasq, Hosts-Clean | ✅ | Stable. Add-ons must be allowed manually |
| **[Adblock-Fast](https://github.com/mossdef-org/adblock-fast)** | Router blocker (OpenWrt only). Works with dnsmasq, SmartDNS and Unbound | Adblock / DNS | ✅ | Stable |
| **[pfSense + pfBlockerNG](https://pfblockerng.com/)** | Firewall / DNS blocker | Adblock / DNS | ⚠️ | Stable. pfSense is not fully open source |
| **[OPNsense](https://opnsense.org/)** | Firewall / DNS blocker (Unbound DNS blocklists) | Domains | ✅ | Stable. Add-ons must be allowed manually |

## 💻 Device-level

### Windows

| Tool | Type | Format | FOSS | Notes |
| ---- | ---- | ------ | :--: | ----- |
| **[Zen Adblocker](https://github.com/irbis-sh/zen-desktop)** | System-wide adblocker | Adblock / DNS | ✅ | Stable |
| **[AdGuard for Windows](https://adguard.com/en/adguard-windows/overview.html)** | System-wide adblocker, DNS filtering option | Adblock / DNS | ❌ | Stable. Paid app |
| **[SwitchHosts](https://github.com/oldj/SwitchHosts)** | Hosts changer and editor | Hosts | ✅ | ⚠️ Unstable |
| **Notepad** | Manual hosts file editing | Hosts | n/a | ⚠️ Be careful |

### Linux

| Tool | Type | Format | FOSS | Notes |
| ---- | ---- | ------ | :--: | ----- |
| **[Zen Adblocker](https://github.com/irbis-sh/zen-desktop)** | System-wide adblocker (GUI) | Adblock / DNS | ✅ | Stable |
| **[OpenSnitch](https://github.com/evilsocket/opensnitch/wiki/block-lists)** | System-wide firewall (GUI), using blocking rules | Hosts | ✅ | Stable |
| **[Hosty](https://github.com/astrovm/hosty)** | Hosts-based blocker (CLI) | Hosts | ✅ | Stable |
| **[AdGuard CLI](https://adguard.com/kb/adguard-for-linux/installation)** | System-wide adblocker and DNS filter (CLI) | Adblock / DNS | ❌ | ⚠️ Unstable. Paid app |
| **`/etc/hosts`** | Manual editing with a terminal text editor | Hosts | n/a | ⚠️ Be careful |

### Android

| Tool | Type | Format | FOSS | Notes |
| ---- | ---- | ------ | :--: | ----- |
| **[BlockAds for Android](https://github.com/pass-with-high-score/blockads-android)** | System-wide adblocker | Hosts, Adblock / DNS | ✅ | Semi-stable. No root: local VPN. Root: local proxy |
| **[AdGuard for Android](https://adguard.com/en/adguard-android/overview.html)** | System-wide adblocker, DNS protection | Adblock / DNS | ❌ | Stable. Paid app. No root: local VPN. Root: local proxy |
| **[personalDNSfilter](https://github.com/IngoZenz/personaldnsfilter)** | DNS filter | Hosts, Domains | ✅ | Stable. No root: local VPN |
| **[AdAway](https://github.com/AdAway/AdAway)** | Hosts-based adblocker | Hosts | ✅ | Stable. Works with or without root (local VPN) |

---

# 📝 Notes on Compatibility

* The **Adblock / DNS** format works perfectly on AdGuard Home.
* **Zen Adblocker** is still early in development, so it can be unstable when enforcing the filters.
* **Hosts** rules work anywhere that supports the hosts format, on any platform.
* I don't know if the Adblock / DNS rules work correctly on **Pi-hole**, specifically the `$important` rules. They work fine on AdGuard Home.
* **pfSense + pfBlockerNG** and **Adblock-Fast** both work with the Adblock / DNS format. Domains and Hosts also work if you prefer them.
* **OPNsense** works best with the Domains format.
* **Adblock-lean on OpenWrt:** Domains, DNSMasq and Hosts-Clean all work (plain `hosts` gives an error). In every case you need to allow the add-on domains manually using the allowlist, since Adblock-lean can't do it automatically.

---

# 🕵️ Mozilla Also Uses Google Trackers

Mozilla's own sites load Google trackers, and they don't let adblockers detect or report them.

**uBlock Origin and uMatrix/nuMatrix can't detect or block** the scripts from `google-analytics.com` and `googletagmanager.com` on Mozilla's site (Mozilla Add-ons) in Firefox and modern Firefox forks. This is because of a policy Mozilla forces onto extension makers, probably with security as the excuse. **AdGuard for Windows and Android** also don't detect the HTTPS Google tracking requests and scripts on Mozilla websites like Mozilla Add-ons, in any browser, even Chrome.

So I don't recommend relying on AdGuard's system-wide adblocker for Firefox or any standard Firefox fork. AdGuard is fine for other browsers. A DNS filter still blocks every tracker without Mozilla's policy getting in the way.

**What about Pale Moon and Basilisk?** Of all the Firefox forks, only unique ones like Pale Moon and Basilisk don't have this policy forced on them. They do suffer from frequent performance and stability issues though. Blocking Mozilla at the system/DNS level and using a modern fork like LibreWolf, Floorp or Zen is better for comfortable day-to-day use.

uBlock Origin Legacy (a uBlock fork) and nuMatrix (a uMatrix fork) can block the Google tracking scripts on Mozilla websites in Pale Moon and Basilisk.

Blocking these Google trackers with a DNS adblocker like AdGuard Home or Pi-hole should be enough to stop the tracking, but it can't stop the scripts from running on Mozilla websites in Firefox and standard Firefox forks. For privacy and security-minded people this can be an issue. Regular users will be just fine blocking Mozilla system-wide with DNS/hosts blocking.

---

# 📚 Useful Resources for Firefox and Firefox-based Browsers

### 1. [HaGeZi DNS Blocklists](https://github.com/hagezi/dns-blocklists)

Currently the best maintained collection of filters for privacy, security, and blocking ads and trackers. A must-have for any blocking system.

I use several HaGeZi filters on my AdGuard Home server, AdGuard for Android, AdAway, and all the adblockers in the browsers I use. For most people, **Pro** and the **Threat Intelligence Feeds** will cover all your ads, tracking, and security concerns. You can use **Ultimate** if you don't mind unblocking specific domains of the services you use.

### 2. [yokoffing filterlists](https://github.com/yokoffing/filterlists)

Recommended for most general users. A balanced set of adblocking and privacy filters for uBlock Origin, AdGuard and Brave.

Just configure your adblocker and enjoy a cleaner, faster internet with most website tracking blocked, without the browser slowdowns some privacy methods cause.

### 3. [Phoenix](https://codeberg.org/celenity/Phoenix)

A suite of configurations and advanced modifications for Mozilla Firefox. Only for people who want maximum privacy. If you care about performance instead, use a good Firefox fork and tweak the browser settings and uBlock Origin filters manually.

It's mostly automated for Linux distros: install it once with your package manager. You can also install official Firefox through your package manager, so you don't need to access Mozilla's servers. On Windows you need access to Mozilla's FTP to download the installer, which I keep blocked because Mozilla also uses FTP URLs for tracking calls. If you won't use Phoenix, just use a Firefox fork.

### 4. [BadBlock](https://codeberg.org/celenity/BadBlock)

A collection of blocklists by celenity (also the author of Phoenix), covering a variety of services, applications and platforms. In celenity's words, it blocks "stuff that is bad™".

A good set of privacy-focused lists that yokoffing doesn't cover. Use them to improve your privacy and security if you're interested.

### 5. [LibreWolf](https://librewolf.net/)

A custom version of Firefox focused on privacy, security and freedom.

Probably the Firefox fork with the least Mozilla tracking out of the box. It still makes a few Mozilla connections, but they're minimal. For privacy-conscious people I'd suggest either **official Firefox + Phoenix** or **LibreWolf + uBlock Origin with yokoffing's filters**. Phoenix for LibreWolf would be wonderful, and I do hope [celenity](https://codeberg.org/celenity) starts supporting LibreWolf alongside Firefox someday.

### 6. [Zen Browser](https://zen-browser.app/)

A trending Firefox fork with tons of features and a sidebar tab layout by default. Currently one of the two best looking and best performing Firefox forks. **Not privacy focused.**

It makes a lot of home calls to the Zen domain. Block `zen-browser.app` and install the browser through your Linux package manager, UniGetUI on Windows (Winget, Chocolatey), or directly from their [GitHub releases](https://github.com/zen-browser/desktop/releases).

### 7. [Floorp Browser](https://floorp.app/)

A good looking, customizable and fast Firefox fork. Many used to call it the Vivaldi of Firefox. **Not privacy focused.**

It's very fast and was a delight to use as my default browser before I switched to Brave. It has lots of customization options, though not as many as Zen. It calls home less than Zen, which is good, but it still does for occasional updates. You can block Floorp domains like `floorp.app` and use a package manager to install and update it, or download the installer from their [GitHub releases](https://github.com/Floorp-Projects/Floorp/releases).

---

# 🔗 All Sources and Mirrors

* **Codeberg:** https://codeberg.org/privacyfilters/Mozilla-Blocker
* **GitHub (mirror):** https://github.com/privacyfilters/Mozilla-Blocker
* **CdnjsDelivr (CDN for the GitHub mirror):** https://cdn.jsdelivr.net/gh/privacyfilters/Mozilla-Blocker@main/