.. _install/installarchive:

===============================
Install Bacula-Web from archive
===============================

Download the source tarball
===========================

Move into Apache directory

On RedHat / Centos

::

   # cd /var/www/html
 
On Debian / Ubuntu

::
   
   # cd /var/www/

::

   # curl -O -L https://www.bacula-web.org/files/bacula-web.org/downloads/bacula-web-latest.tgz

Verify archive signature (optional)
===================================

Download sha256 or sha512 signature file from the download page, and run one of these command to verify the signature

::

   # cat sha256sum.txt | sha256sum -c

   or

   # cat sha512sum.txt | sha512sum -c

Create Bacula-Web folder
========================

**On Centos / Fedora / RHEL**

::

   # mkdir -v /var/www/html/bacula-web
 
**On Debian / Ubuntu**

::

   # mkdir -v /var/www/bacula-web

Decompress the archive
======================

**On Red Hat / Centos / Fedora**

::

   # tar -xzf bacula-web-latest.tgz -C /var/www/html/bacula-web
 
**On Debian / Ubuntu**

::

   # tar -xzf bacula-web-latest.tgz -C /var/www/bacula-web

Change files/folders permissions
================================

**On Centos / Red Hat / RHEL**

::

   # chown -Rv apache: /var/www/html/bacula-web
   # sudo chmod -Rv 755 /var/www/html/bacula-web
 
**On Debian / Ubuntu**

::

   $ sudo chown -Rv www-data: /var/www/bacula-web
   $ sudo chmod -Rv 755 /var/www/bacula-web

It's now time to :ref:`install/configure`
