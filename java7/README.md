Java 7
=========

A simple role to install java-jre 7.x

Requirements
------------

Download the required java tarball from the OTN, and put it in files/ ... I've not included it here for size reasons

Role Variables
--------------

Set the vars correctly for the java version you downloaded. The defaults currently are:

jdkversion: 1.7.0
javaversion: 7
jdkpatch: 67

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: sigio.java7, x: 42 }

License
-------

BSD / MIT

Author Information
------------------

Mark Janssen // Sig-I/O Automatisering
http://sig-io.nl
