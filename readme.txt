=== Purge Varnish Cache ===
Contributors: devavi
Donate link: http://avantikayadav.com/donate.html
Tags: varnish, purge, cache, caching, flush, speed, plugin, wp-cache, performance, fast, automatic
Requires at least: 4.0
Tested up to: 4.8
Stable tag: 1.0.6
License: GPLv2 or later

Automate purge Varnish cache when post content on your site is created or modified and also allow you to purge Varnish cache manually.


== Description ==

Purge Varnish Cache provides integration between your WordPress site and multiple Varnish Cache servers. Purge Varnish Cache sends a PURGE request to the URL of a page or post every time based on configured actions and trigger by site administrator. Varnish is a web application accelerator also known as a caching HTTP reverse proxy.

<strong>Features:</strong>

*   One time configuration.
*   admin-socket integration and Varnish admin interface for status.
*   Purge from N number of Varnish Cache servers
*   Purge custom URLs.
*   Manual Purge.
*   One click purge all.
*   Debugging.

<strong>Requirements:</strong> Apache sockets module/extention should be enabled.

<strong>Purpose:</strong> The main purpose of developing this plugin is to deliver updated copy of content to end user without any delay.

<strong>Enhancement Request:</strong> For any further enhancement, please mail me at <a href="mailto:dev.firoza@gmail.com"><strong>dev.firoza@gmail.com</strong></a>

== Installation ==

<strong>How to install Purge Varnish?</strong>

*   Go to your admin area and select Plugins -> Add new from the menu.
*   Search for "Purge Varnish" or download
*   Click install and then click on activate link.

<strong>How to configure settings?</strong>

*   Access the link DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-settings and configure terminal settings.
*   Access the link DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-expire and configure required actions and events.
*   Access the link DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-urls for purge urls from varnish cache.
*   Access the link DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-all to purge all varnish cache.

== Frequently Asked Questions ==

<strong>How can I check everything's working?</strong>

It is not difficult. Install this plugin and configure Terminal settings using below link.
DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-settings. 

If status is 'Varnish running' means everything is working perfectly!

<strong>What versions of Varnish is supported?</strong>

Currently it is supporting all varnish versions of 3.x, 4.x, 5.x

<strong>How do I manually purge a single URL from varnish cache?</strong>

Click on 'Purge URLs' link or access below link.
DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-urls.

<strong>What if I have multiple varnish Servers/IPs?</strong>

You need to configure multiple IPs in Varnish Control Terminal textfield in 'Terminal' screen like 127.0.0.1:6082 127.0.0.2:6082 127.0.0.3:6082

<strong>How can I debug?</strong>

Add below constant in wp-config.php file.
<strong>define('WP_VARNISH_PURGE_DEBUG', true);</strong>

It will generate a log file 'purge_varnish_log.txt' inside uploads directory.

<strong>How do I manually purge the whole site cache?</strong>

Clicking on link 'Purge all' or access below link: 
DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-all.

<strong>What it purge?</strong>

It allow you to configure purge settings.
Please configure by clicking on Expire link or accessing below link.
DOMAIN_NAME/wp-admin/admin.php?page=purge-varnish-expire to configure purge expire setting.Clicking on Expire link 



== Screenshots ==

1. Terminal settings screen for test connectivity from varnish server. 

2. Action trigger configuration screen to make automate purge varnish cache for post expiration.

3. Action trigger configuration screen to make automate purge varnish cache for comment expiration.

4. Action trigger configuration screen to make automate purge varnish cache on menu update.

5. Action trigger configuration screen to make automate purge varnish cache on theme change.

6. Purge whole site cache.

7. Purge URLs screen to purge URLs manually from varnish cache. 


== ChangeLog ==

= 1.0.6 =

Implement Trigger to purge/post on comment approved/unapproved
Fix: Wrong number of arguments
Update screens.

= 1.0.5 =

Purge Custom URLs
Update screens.

= 1.0.4 =

Enable expire configuration automatically when plug in enabled.
Add more tags.
Update screens.

= Version 2.x =

* PHP 4.x/5.x/6.x/7.x compatibility.

== Upgrade notice ==
....