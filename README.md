# Block-Spotify-ADS-DNS-List
A dentist blocking list for blocking Spotify ads.. 

```markdown
# 🎧 Spotify Ads DNS Blocklist

A powerful DNS blocklist to remove Spotify ads and tracking services. This list includes domains used by Spotify to deliver audio ads and collect tracking data. By adding this list to your DNS blocker (Pi-hole, AdGuard Home, or NextDNS), you can enjoy a cleaner Spotify experience without interruptions.

---

## 🚀 How It Works

Spotify serves ads through specific domains. By blocking these domains, the ads will not be served, which can result in an ad-free experience. This list focuses on blocking:
- **Ad-serving domains**: Prevents Spotify from delivering audio ads.
- **Tracking domains**: Blocks services that collect analytics and user behavior data.

> ⚠️ **Disclaimer**: Using this blocklist may violate Spotify’s terms of service. Use at your own risk. Blocking too aggressively may cause issues with the app, such as playback problems or incomplete functionality.

---

## 📦 How to Use

### 🔹 Pi-hole Setup

1. Open your Pi-hole Admin interface.
2. Navigate to **Group Management > Adlists**.
3. Copy the blocklist from the [Blocklist](#blocklist) section and paste it as a new entry.
4. After adding the blocklist, update the gravity list by running:
   ```bash
   pihole -g
   ```
5. Finally, restart your DNS resolver for changes to take effect:
   ```bash
   sudo systemctl restart pihole-FTL
   ```

### 🔹 AdGuard Home Setup

1. Open your AdGuard Home dashboard.
2. Navigate to the **Filters** section.
3. Click **Add Custom Filtering Rule** and paste the blocklist from the [Blocklist](#blocklist).
4. Save and apply changes to begin blocking Spotify ads.

### 🔹 NextDNS Setup

1. Log in to your [NextDNS Dashboard](https://my.nextdns.io).
2. Go to the **Allowlist/Blocklist** tab.
3. Paste the blocklist from the [Blocklist](#blocklist) section into the Blocklist area.
4. Save your changes and apply the configuration to your NextDNS setup.

---

## 📜 Blocklist

Below is the list of domains to block. Copy this list and add it to your DNS blocker as explained in the instructions.

```
audio-ads.spotify.com
adclick.g.doubleclick.net
pubads.g.doubleclick.net
spclient.wg.spotify.com
heads-ec.spotify.com
ads-fa.spotify.com
adeventtracker.spotify.com
pagead46.l.doubleclick.net
securepubads.g.doubleclick.net
googleads.g.doubleclick.net
www.googletagservices.com
www.googleadservices.com
tpc.googlesyndication.com
pagead2.googlesyndication.com
stats.g.doubleclick.net
ads.g.doubleclick.net
googlesyndication.com
s0.2mdn.net
static.doubleclick.net
crashlytics.com
metrics.spotify.com
log.spotify.com
google-analytics.com
ssl.google-analytics.com
analytics.google.com
ads.yahoo.com
ads-twitter.com
ads.linkedin.com
ads.facebook.com
secure.adnxs.com
ib.adnxs.com
adservice.google.com
adservice.google.co
```

---

## ⚙️ How to Set It Up

### Requirements
- A DNS blocker (e.g., Pi-hole, AdGuard Home, or NextDNS)
- Access to your DNS blocker's admin panel or dashboard

### Steps
1. **Copy the Blocklist**: Get the list of domains from the [Blocklist](#blocklist) section.
2. **Add the Blocklist**: Paste it into your DNS blocker's adlist, filtering rule, or blocklist section.
3. **Apply Changes**: Ensure the changes take effect by updating the gravity list or applying your DNS configuration.
4. **Test It**: Open Spotify and ensure no ads are being played. If Spotify experiences issues, you may need to review your blocklist to ensure you aren't blocking essential domains.

---

## 🔄 Updates & Maintenance

- Spotify frequently updates its ad-serving domains. This blocklist will be maintained and updated regularly to ensure continued functionality.
- Check back for updates or watch this repository to stay informed of changes.
- If you notice new ads, feel free to contribute by suggesting new domains to block.

---

## ❗ Disclaimer

- **Use at your own risk**: Blocking ads may violate Spotify’s terms of service.
- **Support artists**: Ads are a primary source of revenue for artists on Spotify, and by blocking ads, you reduce their earnings.
- **App malfunctions**: Blocking too many domains could result in incomplete functionality within the app.

---
```

### Key Features:
1. **How It Works**: Explains the purpose of the blocklist.
2. **How to Use**: Step-by-step guides for Pi-hole, AdGuard Home, and NextDNS setup.
3. **Blocklist**: Clear and easy-to-copy list of domains.
4. **How to Set It Up**: A section for easy setup instructions, with requirements and a step-by-step overview.
5. **Updates & Maintenance**: Encourages users to check back for updates or contribute to the blocklist.
6. **Disclaimer**: Provides legal and ethical context for users.

This version provides a clear, structured, and user-friendly GitHub README. You can copy and paste this into your repository's `README.md` file.
