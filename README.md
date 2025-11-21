# ebay-dropship-woocommerce
A fully autonomous and robust open-source WordPress plugin for eBay dropshipping. Automates price/stock sync, order placement, tracking updates, and features API rate limiting.
📦 eBay Automated Dropship Plugin for WooCommerce

✨ Overview

The eBay Automated Dropship Plugin is an open-source solution designed to seamlessly link eBay listings to a WooCommerce store, automating the entire dropshipping fulfillment lifecycle. This plugin allows store owners to focus on marketing and sales while delegating the tedious tasks of price syncing, stock monitoring, and order placement to the software.

It adheres to high standards of reliability by incorporating API Rate Limiting, Exponential Backoff, and Automatic Token Refresh to ensure 24/7 autonomous operation.

🚀 Key Features

🛒 Automated Product Import: Search, filter, and bulk import eBay listings directly into WooCommerce as draft products, automatically fetching images, titles, and descriptions.

🔄 Live Price and Stock Sync: A daily scheduled task automatically checks the source eBay listing. It adjusts your WooCommerce price (based on your set markup of 15%) and updates stock quantity.

🛡️ Listing Health Monitor: Critical automation that detects listings that have been removed, ended, or gone out of stock on eBay, automatically delisting the corresponding WooCommerce product (setting it to Draft) and notifying the admin.

🚢 Autonomous Order Fulfillment: When a customer places a paid order on your WooCommerce site:

The plugin automatically initiates a fulfillment order with the source eBay seller via API.

A separate sync job periodically checks the fulfillment status.

Once the source seller ships the item, the plugin fetches the tracking number and automatically updates the WooCommerce order status to "Completed," notifying the customer.

🔒 Stable API Connection: Includes Token Refresh Logic and API Rate Limiting with Retries to prevent connection failures and service interruption.

🗄️ Database Logging: All critical events (sync errors, fulfillment failures, delisting actions) are recorded in a custom database log for easy diagnosis.

🛠️ Installation and Setup

Prerequisites

WooCommerce must be installed and active.

An eBay Developer Account with a registered application to obtain your Client ID (App ID) and Client Secret (Cert ID).

Steps

Download: Download the latest release ZIP file of the plugin.

Upload: In your WordPress admin, go to Plugins > Add New > Upload Plugin and select the ZIP file.

Activate: Activate the eBay Automated Dropship plugin.

Configure Credentials: Navigate to eBay Dropship > Settings in the admin menu.

Enter your Client ID and Client Secret.

Click "Save Changes."

Authorize Connection: Click the "Connect & Authorize eBay" button. This will redirect you to eBay for permission. Grant access, and you will be returned to your dashboard with a successful connection status.

🤝 Contribution Guidelines

This project is built for the open-source community! Contributions, issues, and feature requests are highly welcome. The complete history of the design and coding decisions is archived in the DEVELOPMENT_LOG.md file (or the external Paste.ee link).

How to Contribute

Fork the repository.

Create a new branch for your feature or fix (e.g., feature/add-category-mapping).

Code your changes, adhering to WordPress coding standards.

Ensure all new features are covered by basic logging (using Ebay_DS_Logger).

Commit your changes and open a Pull Request describing your changes in detail.

📄 License

This project is licensed under the GNU General Public License v3.0 (GPLv3). Please see the LICENSE.txt file for full details.
