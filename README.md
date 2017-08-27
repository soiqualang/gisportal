Web portal for QGIS projects published by EQWC
==============================================

This is start page - Web portal for browsing and opening QGIS projects published with [Extended QGIS Web Client.](https://github.com/uprel/gisapp)
User registration and login is now part of this. Next steps are planned to have complete web administration part for publishing projects and layers,
delegating user permissions...

Built with Codeigniter and Bootstrap.

## Setup

You go through this after you setup EQWC!

1. Checkout into web root to have gisportal folder beside gisapp folder (EQWC)
2. Setup database connection in application/config/database.php
3. Setup base_site and other EQWC settings at bottom of application/config/config.php
4. Edit header_logo.png in assets/img folder
5. To preserve session information from gisapp to gisportal you have to edit php.ini and change line

session.name = PHPSESSID
to
session.name = sess_

This means that you login to gisportal and then browse all public projects or projects you have permission without
new login.

6. Email service
If you entered correct gmail info at the bottom of config.php you enabled email service. This service can be used to sending
emails from gisapp or gisportal.

[Test mail - localhost example](http://localhost/gisportal/index.php/mail/test)

Email service is currently used with new User Feedback control in gisapp and with Editor plugin.
It is planned to be used with gisportal (for sending emails to users) and for other tasks in gisapp.

## Thumbnail images

gisportal uses thumbnail images for client and project display. Copy images to assets/img/clients or assets/img/projects
folder with client or project alis as name and in PNG format.

## Support

Contact us for:
* support
* custom development

Uroš Preložnik, http://level2.si
