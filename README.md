Accounts-Linkblue
==
##Overview##
This is a package to implement LDAP authentication with the UK LDAP servers in Meteor.js. 

##Installation##

Since this is a private package, there is currently no way to publish on the new meteor packaging system privately. 
To test the package, create a packages/ directory in your meteor app, and move hive:accounts-linkblue there. Then add a line containing hive:accounts-linkblue in .meteor/packages and run your app.

* mkdir -p packages
* git clone https://github.com/UK-AS-HIVE/meteor-accounts-linkblue packages/hive:accounts-linkblue
* meteor add hive:accounts-linkblue

##Usage##
{{> linkblueLogin}} renders a template with username and password inputs. If login is successful, user will be added to Meteor.users(). It is up to the app to publish and subscribe fields. By default only the username is published.

To run example:
- cd hive:accounts-linkblue/examples/basic
- meteor run
