Tomcat 7
=========

A simple role to download and install Apache Tomcat 7

Requirements
------------

Java-7, installed in /opt/java7... like from the sigio.java7 role

Role Variables
--------------

The vars file contains the download server, tomcat-version requested, and sha256sum of the download file.
You can also specify the installation directory, and the name of the unversioned symlink.a

Default values:

dlsite: 'http://ftp.nluug.nl/internet/apache/tomcat/tomcat-7/'
dlurl: '{{ dlsite }}/v{{version}}/bin/apache-tomcat-{{version}}.tar.gz'
version: '7.0.55'
shasum: 'c20934fda63bc7311e2d8e067d67f886890c8be72280425c5f6f8fdd7a376c15'
tomcatuser: tomcat6
installroot: /opt
installsymlink: tomcat7

Dependencies
------------

Depends on sigio.java7

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: sigio.tomcat7 }

License
-------

BSD

Author Information
------------------

Mark Janssen // Sig-I/O Automatisering
http://sig-io.nl
