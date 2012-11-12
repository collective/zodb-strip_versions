ZODB strip_versions
===================

Buildout for stripping out version data from ZODB files.

Until ZODB version 3.8, version data was kept in ZODB storages. Since ZODB
version 3.9, version data support was removed. The Zeo server and Zope won't
start with old storages, failing with

    ValueError: Non-zero version length. Versions aren't supported.

Use this buildout to remove version data from ZODB storages.

Usage
-----

$ ./bin/strip_versions PATH-TO-OLD-ZODB-FILE PATH-TO-NEW-ZODB-FILE


Authors
-------

Chris Withers, Johannes Raggam. Based on:
https://mail.zope.org/pipermail/zodb-dev/2009-August/012690.html

Also see
--------

[ZODB-Dev] "Versions aren't supported" message in Plone 4 upgrade
https://mail.zope.org/pipermail/zodb-dev/2010-September/013618.html

[ZODB-Dev] Stripping version data from databases
https://mail.zope.org/pipermail/zodb-dev/2010-September/013621.html
