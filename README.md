# drupal-opengraph

This module allows any page to be marked up with Facebook's Open Graph meta data. 
A page requires this meta data for effective use of the Like button and other social plugins 
For more information on the Open Graph protocol see http://opengraphprotocol.org 

This module is released under the GNU General Public License, version 2. 
http://www.gnu.org/licenses/gpl-2.0.txt 

This version of the module only works with Drupal 6.x. 


## INSTALL 

This module installs a single `opengraph` table which holds open graph properties against node ids. 
Make sure your HTML page tempate has namespaces as follows: 
<html 
  xmlns="http://www.w3.org/1999/xhtml" 
  xmlns:fb="http://www.facebook.com/2008/fbml" 
  xmlns:og="http://opengraphprotocol.org/schema/">

Go straight to the settings page to configure your node types and default properties:
 admin/content/opengraph


## FEATURES 

Adds Open Graph protcol meta tags in the HTML head of all pages. 
Check HTML head source to see the output of the module. 

Makes a single block available which displays the standard Like button 

Default properties can be set in the admin screen at admin/content/opengraph. 
Individual nodes may override the default settings in the node edit form. 
Additionally some values are guessed when there are no settings, for example when a page is not a node. 


## TODO

* Blocks for other social plugins
* image file cleanup
* provide hooks for other modules to set properties when page is not a node
* improve theming and configuration of like block
