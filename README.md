# Copelandia

Copelandia is a proof of concept for a [COPE]
(http://blog.programmableweb.com/2009/10/13/cope-create-once-publish-everywhere/)
oriented Drupal site, to decouple the Drupal Backend from the Frontend.

## INSTALLATION

1. Clone this repository's project.
1. Set up a local virtualhost, such as copelandia.local pointing to root-of-this-project/docroot.
 * Also add the entry at your hosts file.
1. Install the site by going to http://copelandia.local/install.php
 * You can also install Drupal via Drush.
1. Enable the following modules: copelandia, copelandiarecipes, copelandia_rest.
1. Open http://copelandia.local in your browser. You should get the same output as the one at
http://copelandia.lulladev.com.
1. Create some recipes.

## OAuth authentication
Some of the client requests need OAuth authentication. For example, registering a user or
submitting a request. Here is how to set up OAuth keys so a client website can submit
authenticated requests to this site.

1. Log in as administrator.
1. Edit a user and open the tab "OAuth consumers".
1. Click on "Add a consumer"
1. Give it a name and click Save (leave callback blank and the Application context as "copelandia".
1. Use the Application Key and Application Secret credentials to authenticate your requests.
