# Introduction #

This is a minimalistic tutorial on how to get the framework up and running. Build instructions for individual packages are generally provided in the INSTALL file of each project. We will focus here on suggesting a list of packages to check out and the order in which they must be built.

# Building order #

First build the core packages:
  * [libaccounts-glib](http://code.google.com/p/accounts-sso/source/list?repo=libaccounts-glib)
  * [libaccounts-qt](http://code.google.com/p/accounts-sso/source/list?repo=libaccounts-qt)
  * [signond](http://code.google.com/p/accounts-sso/source/list?repo=signond)
  * http://code.google.com/p/accounts-sso/source/list?repo=libsignon-glib

Then, build the authentication plugins which you are going to use:
  * [signon-plugin-oauth](http://code.google.com/p/accounts-sso/source/list?repo=signon-plugin-oauth2)
  * There are more plugins available from the project repositories, but they are not essential to try out the project

The service which handles the UI is not strictly required, but it's essential for those authentication methods which rely on user interaction, such as OAuth:
  * [signon-ui](https://launchpad.net/online-accounts-signon-ui): this is the Ubuntu Online Accounts implementation; other implementations are also possible.

In order to get some data files for the account providers and services, plus a command-line tool which allows to test out the accounts and the authentication, it's recommended to install these projects:
  * [gnome-control-center](https://launchpad.net/online-accounts-gnome-control-center): Online Accounts panel for the GNOME control center.
  * [account-plugins](https://launchpad.net/online-accounts-account-plugins): Account plugins (XML files and binary plugins for the control center) and `account-console` command-line tool.