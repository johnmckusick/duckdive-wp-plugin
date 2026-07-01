# DuckDive Attribution for WordPress

**First-party marketing attribution for WordPress** — see where your leads came from, automatically.

DuckDive captures referrer, UTM parameters, and ad click IDs when visitors land on your site, then attaches that data to form submissions. Everything is stored in your WordPress database under **DuckDive → Leads**.

Learn more at **[duckdive.ai](https://duckdive.ai)**.

## Install or update

1. Download the latest **`duckdive-attribution.zip`** from **[Releases](https://github.com/johnmckusick/duckdive-wp-plugin/releases)**.
2. In WordPress, go to **Plugins → Add New → Upload Plugin** (or update from the Plugins screen if auto-updates are enabled).
3. Activate the plugin.

No extra setup is required for form tracking — supported form builders are tracked automatically.

## What you get

- **Automatic form capture** — Elementor, HubSpot, Go High Level, Contact Form 7, Gravity Forms, WPForms, and standard HTML forms
- **Multi-touch journey** — first touch, last touch, and full visit history
- **Click ID support** — Google Ads (`gclid`), Meta (`fbclid`), Microsoft (`msclkid`), LinkedIn, TikTok, Yahoo, and more
- **UTM tracking** — campaign, source, medium, term, content
- **Lead dashboard** — view and export leads with attribution in WordPress admin
- **First-party tracking** — uses browser storage on your domain (no third-party ad cookies)

## Settings

Go to **DuckDive → Settings** in WordPress admin:

| Setting | What it does |
|---------|----------------|
| **Attribution window** | How long visitor attribution is remembered (default 30 days) |
| **DuckDive API key** | Unlocks advanced referrer labels (Google, Facebook, ChatGPT, etc.). Request a key at [duckdive.ai](https://duckdive.ai) or email [hello@duckdive.ai](mailto:hello@duckdive.ai) |
| **Google Sheets** | Optional export of leads to a spreadsheet (requires API key) |

Your API key is tied to your website domain. If you add staging or new domains, contact [hello@duckdive.ai](mailto:hello@duckdive.ai).

## Automatic updates

If your host supports it (for example **WP Engine Smart Plugin Manager**), WordPress will show **Update available** when a new version is published here. No GitHub account is required on your site.

## Support

- Website: [duckdive.ai](https://duckdive.ai)
- Email: [hello@duckdive.ai](mailto:hello@duckdive.ai)

## License

This plugin is **proprietary software**. Use is limited to authorized DuckDive customers and licensed websites. See [LICENSE](LICENSE) for terms.
