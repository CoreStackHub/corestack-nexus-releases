# CoreStack Nexus

CoreStack Nexus is a commercially licensed investment operations platform for managing investor accounts, funding activity, structured investment products, automated trading strategies, verification workflows, communications, and administrative operations from one system.

> CoreStack Nexus is proprietary software. Possession of the files does not grant permission to use, copy, resell, redistribute, sublicense, or publish the software. A valid commercial license is required.

## Platform Highlights

- Investor dashboards, profiles, account activity, and portfolio views
- Manual and provider-assisted deposit workflows
- Withdrawal requests, configurable policies, and portfolio tiers
- AI bot strategy plans with risk labels, trading access limits, cooldowns, and account-specific controls
- Structured investment products with configurable performance behavior
- KYC submission and administrative review
- Database-backed mail templates, notifications, delivery logs, and newsletter preferences
- Public CMS pages, multilingual public and investor experiences, and due-diligence resources
- Support inbox, live-chat controls, and configurable contact channels
- Browser-based installer and resumable shared-hosting updater
- Installable progressive web app support for compatible mobile and desktop browsers

## Hosting Requirements

| Requirement | Minimum | Recommended |
| --- | --- | --- |
| PHP | 8.2 | PHP 8.3 with OPcache |
| Database | MySQL 8.0 or MariaDB 10.6 | Current stable MySQL or MariaDB |
| Web server | Apache, LiteSpeed, or Nginx | Managed hosting with HTTPS |
| PHP memory | 256 MB | 512 MB or more |

Required PHP extensions: `bcmath`, `ctype`, `curl`, `dom`, `fileinfo`, `json`, `mbstring`, `openssl`, `pdo`, `pdo_mysql`, `tokenizer`, `xml`, and `zip`.

Supported environments include cPanel, Plesk, DirectAdmin, CyberPanel, managed VPS panels, and conventional Apache/Nginx hosting that meets the requirements above.

## Installation

Use the packaged release, not the source repository checkout.

1. Download the current `CoreStack-Nexus-...zip` install package from the release supplied with your purchase.
2. Extract the package and open `Documentation/index.html` for the complete customer installation guide.
3. Upload the contents of `CoreStack-Nexus-Files` to the hosting location assigned to your domain.
4. Point the domain document root to `public` when your hosting panel supports it. The documentation includes a `public_html` fallback for shared hosting.
5. Visit `https://your-domain.com/install` and complete the browser-based installer.
6. Configure real payment addresses, SMTP, cron, support channels, branding, and live-chat settings after signing in as the administrator.

Do not browse to `/public/install`. If `/install` returns 404, verify the extraction folder, hidden `.htaccess` file, and domain document root.

## Updating

Existing installations should use the matching `-upgrade.zip` through:

`Admin Settings > Update Center`

Back up the database and application files before every update. Do not manually overwrite `.env`, `storage`, `public/storage`, or administrator-uploaded assets.

## Documentation

The customer package includes an offline HTML guide at `Documentation/index.html`. It covers:

- shared-hosting and control-panel deployment
- folder permissions
- database and mail configuration
- cron and queue setup
- installation troubleshooting
- post-install security checks
- upgrades and backups

## Security

- Serve the application over HTTPS.
- Keep `.env`, storage data, database exports, and license credentials private.
- Replace all demo configuration before production use.
- Use strong administrator credentials and enable available account security controls.
- Apply supported releases through the Update Center.

Security concerns should be reported privately through the support channel attached to your commercial purchase. Do not publish sensitive findings in a public issue.

## Commercial License

CoreStack Nexus is distributed under the [CoreStack Nexus Proprietary Commercial License](LICENSE). It is not open-source or freeware. A purchase or issued license key grants only the rights stated in the applicable order, license agreement, and the included license notice.

Laravel and other third-party dependencies remain subject to their respective licenses.

Copyright (c) 2026 CoreStack. All rights reserved.
