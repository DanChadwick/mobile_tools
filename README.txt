$id:
README.txt
==========
The purpose of this module is to provide de Drupal developer with some tools that assist in making a site mobile.

Main functinalities are:
 - theme switching 
 - User notification (notify users of existence of mobile or desktop site)
 - User redirection (mobile user to the mobile site)
 - Mobile permissions
 - managing the number of displayed posts on the frontpage

This module is designed to work together with the Siruna (http://www.drupal.org/project/siruna) module.

MORE INFORMATION AND SHOWCASES CAN BE FOUND AT http://www.mobiledrupal.com

AGGRESSIVE CACHING
==================
The Mobile Tools module does not support device detection when you use aggressive caching. 
Aggressive cachig bypasses any Drupal loading and by consequence the device detection system.

Recommended is to try user agent detection in your caching server and use a similar algorithm than 
the one used by Mobile Tools. 


AUTHOR/MAINTAINER
======================
Tom Deryckere
Tom DOT Deryckere at siruna DOT com 
http://twitter.com/twitter