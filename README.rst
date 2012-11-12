ZODB strip_versions
===================

Buildout for stripping out version data from ZODB files.

Since ZODB version 3.9, no version data is kept in ZODB storages and zeoserver
or Zope won't start, failing with

    ValueError: Non-zero version length. Versions aren't supported.

Use this buildout to remove version data from ZODB storages.

Usage
-----

$ ./bin/strip_versions PATH-TO-OLD-ZODB-FILE PATH-TO-NEW-ZODB-FILE


Authors
-------

Johannes Raggam, based on Chris Withers' version:
https://mail.zope.org/pipermail/zodb-dev/2009-August/012690.html

Also see
--------

[ZODB-Dev] "Versions aren't supported" message in Plone 4 upgrade
https://mail.zope.org/pipermail/zodb-dev/2010-September/013618.html

[ZODB-Dev] Stripping version data from databases
https://mail.zope.org/pipermail/zodb-dev/2010-September/013621.html
