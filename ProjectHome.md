Accounts and SSO (Single Sign-On) framework for Linux and POSIX based platforms.

# Introduction #

The **Accounts & SSO framework** consists of a set of components and libraries which implement an account manager for a user's online accounts and a single-sign-on daemon which handles the authentication to the remote services on behalf of the client applications.

This software was initially developed for embedded devices as part of the [Meego](http://en.wikipedia.org/wiki/MeeGo) Linux-based platform with a special attention to performance and security. Its high modularity has made it possible to deploy it in very different Linux machines, **from smartphones to desktop computers**, working with diverse user interface technologies and designs, storage back-ends and varying levels of security — yet always providing the **same client API** to applications.


# Client libraries #

All of the client APIs are available in two flavours: one `GLib`-based for C and Python applications, and one `Qt`-based for C++ ones.

The API to access the accounts database is provided by `libaccounts`:
  * [libaccounts-glib API documentation](http://docs.accounts-sso.googlecode.com/git/libaccounts-glib/html/index.html)
  * [libaccounts-qt API documentation](http://docs.accounts-sso.googlecode.com/git/libaccounts-qt/html/index.html)

The API to perform the authentication is provided by `libsignon`:
  * [libsignon-glib API documentation](http://docs.accounts-sso.googlecode.com/git/libsignon-glib/html/index.html)
  * [libsignon-qt API documentation](http://docs.accounts-sso.googlecode.com/git/libsignon-qt/html/index.html)


# gSSO spin-off #

gSSO is a glib-based reimplementation of the single sign-on daemon and authentication plugins with advanced access control and other improvements. The original SSO daemon is written using Qt.

gSSO's homepage is https://01.org/gsso/ and all links to the source code and documentation can be found from there. The project is sharing the issue tracker, the IRC channel and the mailing lists with the original SSO.