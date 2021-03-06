**********************************************************************
Remotes
**********************************************************************


.. autoattribute:: pygit2.Repository.remotes
.. automethod:: pygit2.Repository.create_remote


The Remote type
====================

.. autoclass:: pygit2.Remote
   :members:

The TransferProgress type
===========================

This class contains the data which is available to us during a fetch.

.. autoclass:: pygit2.remote.TransferProgress
   :members:

The Refspec type
===================

.. autoclass:: pygit2.refspec.Refspec
   :members:

Credentials
================

.. automethod:: pygit2.Remote.credentials

There are two types of credentials: username/password and SSH key
pairs. Both :py:class:`pygit2.UserPass` and :py:class:`pygit2.Keypair`
are callable objects, with the appropriate signature for the
credentials callback. They will ignore all the arguments and return
themselves. This is useful for scripts where the credentials are known
ahead of time. More complete interfaces would want to look up in their
keychain or ask the user for the data to use in the credentials.

.. autoclass:: pygit2.UserPass
.. autoclass:: pygit2.Keypair
