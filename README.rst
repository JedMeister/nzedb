nZEDb - Usenet indexer
======================

'nZEDb'_ automatically scans usenet, similar to the way google search 
bots scan the internet. It does this by collecting usenet headers and 
temporarily storing them in a database until they can be collated into 
posts/releases. It provides a web-based front-end providing search, 
browse, and programmable (API) functionality.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- nZEDb configurations:
   
   - Installed from upstream git source code to /var/www/nzedb

     **Security note**: Updates to the nZEDb software will need to be 
     done manually and **ARE NOT** installed automatically.

- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port
  12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e.g.,
  password recovery).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL, Adminer: username **root**
-  nZEDb: username **admin**

.. _nZEDb: http://nzedb.com/
.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _Adminer: http://www.adminer.org/
