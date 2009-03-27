README.txt
==========
The purpose of this module is to provide de Drupal developer with some tools that assist in making a site mobile and choose what content and functionality is beeing shown to the mobile user. These tools are complementary to the existence of a mobile theme or the usage of content adaptation engine.

This functionality of the module contains:
  - User Agent detection ('mobile' or 'desktop')
  - automatic redirection towards mobile site or user notification by means of a block message or drupal_set_message()
  - Adding a mobile context to the permission system
  - Adding a mobile context to theming (= theme switching or seperate configuration for desktop and mobile site)     
  - Change the default frontpage
  
The module provides hooks for other modules that can override device detection or site type detection functionality:
   - hook_is_mobile_device() returns 'mobile' when accessed by a mobile device or 'desktop' in case of a desktop site. The Mobile Tools module has a standard implementations. Third party modules could query databases (e.g. deviceatlas, handsetdetection.com  ) 
   - hook_is_mobile_site() returns true when Drupal is being prepared for display a mobile device. This can be just the selection of a mobile theme, of transcoding. 

A. REDIRECTION and NOTIFICATION
===============================
The module allows automatic redirection to the mobile site or the notification of the existence of a mobile site in case a mobile user visits the site. It is a good practise to give the visitor the option what version he wants to see.
Two type of notification message can be displayed:
 - notification in a block 
 - message on top of the content
 
The number of times the message is being displayed is configurable 

B. MOBILE CONTEXT FOR THE PERMISSON SYSTEM
==========================================
The module gives the administrator the possibility to give mobile users a mobile user role. This way the Drupal permission system can be used to allow or forbid access to mobile users. e.g.: mobile contact page versus desktop contact page.

C. MOBILE CONTEXT FOR THE THEMING SYSTEM
========================================
By enabling the mobile context for the theming, the adminstrator can choose which theme can be showed for display on a mobile device.

If an adaptation engine like http://open.siruna.org is beeing used, the existing desktop theme can be reused by copying the theme in the themes directory and rename the folder and .info file (e.g. copy Garland and rename to mobile-garland
and garland.info to mobile-garland.info.)

MORE INFORMATION AND SHOWCASES CAN BE FOUND AT http://www.mobiledrupal.com

AUTHOR/MAINTAINER
======================
Tom Deryckere
Tom DOT Deryckere at siruna DOT com 