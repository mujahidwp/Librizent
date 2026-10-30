<h1 align="center">Librizent – Media Library Health</h1>

<p align="center"><b>Media Library health audit for WordPress: missing ALT text, oversized and heavy images, broken metadata.</b></p>

<p align="center">
  <a href="https://wordpress.org/plugins/librizent-media-library-health/"><img src="assets/download-wporg.svg" alt="Download on WordPress.org" height="36"></a>
</p>

<p align="center">Free WordPress plugin · Version 1.0.2 · GPLv2 or later</p>

> [!NOTE]
> Librizent – Media Library Health is officially distributed through **WordPress.org**. Please download, install and get updates from its [WordPress.org page](https://wordpress.org/plugins/librizent-media-library-health/) so you always have the latest reviewed version.

## About

Librizent is a lightweight Media Library health and audit plugin. It helps site owners find review-worthy media issues before they become website problems.

Librizent is not an image optimization plugin. It does not compress, replace, rename, or automatically delete media. It does not automatically write ALT text.

The workflow is deliberately safe: **Scan → Review → Decide**.

#### Features

- Media Health Score calculated from actual scan results.
- Missing ALT text detection for images with completely empty ALT values.
- Oversized image detection with a configurable pixel threshold.
- Heavy image file-size detection with a configurable per-image MB threshold.
- Missing or incomplete image dimension metadata detection.
- Missing or unreadable local attachment file detection, with an offloaded-media caution.
- Potentially poor filename detection using conservative filename patterns.
- Possible duplicate detection using SHA-256 hashes where practical and metadata signatures as a fallback.
- Possibly Unused Media review using WordPress-native attachment, featured-image, and content-reference checks.
- Manual ALT text editing with capability and nonce checks.
- Batched manual scanning designed to avoid loading the full Media Library into memory.
- Batch-built usage index so post-content and featured-image checks are not repeated once per attachment.
- Dedicated Media Usage workspace with Usage Found, Possibly Unused, and live attachment review states.
- Scan History with up to 10 compact local summaries, score trends, issue totals, and scan duration.
- Five focused admin destinations: Dashboard, Media Health, Media Usage, Scan History, and Settings.
- No external services, registration, API keys, telemetry, tracking, or AI features.

#### Important safety note about unused media

Librizent intentionally uses the wording **Possibly Unused**. A WordPress media item can be referenced from custom fields, theme options, page builders, CSS, JavaScript, WooCommerce data, or external integrations that this scanner cannot prove exhaustively.

Always review media in context before deleting it. Librizent does not provide automatic deletion.

#### Health Score

The Media Health Score starts at 100. Each issue category has a maximum weight. The deduction for that category is proportional to the share of eligible media affected, capped at the category’s maximum weight.

The score breakdown is shown in the admin so users can see exactly why the score changed.

### Privacy

Librizent works locally inside your WordPress installation. It does not send Media Library data, scan results, site information, or user information to external servers. It does not use telemetry, tracking, remote APIs, external fonts, or third-party JavaScript/CSS services.

The plugin stores its settings, the latest scan state/results, and up to 10 compact scan-history summaries in WordPress options. These plugin-owned options are removed by the included uninstall routine when the plugin is deleted through WordPress.

## Requirements

- WordPress 6.4 or higher
- Tested up to WordPress 7.1.4
- PHP 7.4 or higher

## How to install

1. In your WordPress dashboard go to **Plugins → Add New Plugin**.
2. Search for **Librizent**.
3. Click **Install Now**, then **Activate**.

Or download it directly from **[WordPress.org](https://wordpress.org/plugins/librizent-media-library-health/)**.

## Support

Questions or problems? Please use the **[support forum on WordPress.org](https://wordpress.org/support/plugin/librizent-media-library-health/)**.

## Author

Developed by **[Muhammad Mujahid Sarfraz](https://profiles.wordpress.org/mujahidwp/)** · [All my WordPress products](https://profiles.wordpress.org/mujahidwp/) · [LinkedIn](https://www.linkedin.com/in/muhammad-mujahid-sarfraz-2631a43b6)
