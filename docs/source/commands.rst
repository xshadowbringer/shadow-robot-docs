Commands
=====

.. _administrator:

Administrator
------------

- **Addstock command** | store items to you database

.. code-block:: console

   (syntax) /addstock

- **config command** | create and configurate a database

.. code-block:: console

   (syntax) /config or $config
   
**USAGE**

if you database limit is not reached you will have to follow 4 steps :

>>>1. Enter channels ID's that receiving an item is allowed
>>>2. Enter roles ID's that are allowed to see the current stock of the item
>>>3. Enter channels ID's that seeing the current items stock is allowed
>>>4. Enter the channel ID of the log channel, that will print the receivings

- **databases command** | show all databases and their settings

.. code-block:: console
   
   (syntax) /databases {database_id} or $databases {database_id}
  
- **items command** | available to PRO Version see  :doc:`pro-features`

- **reconfig command** | edit your database settings

.. code-block:: console

   (syntax) /reconfig {database_id} {setting} or $reconfig {database_id} {setting}
   
setting can be one of those : ``gen_channels`` | ``allowed_roles`` | ``stock_channels`` | ``log_channel``

- **unstock command** | drop a category from your database

.. code-block:: console

   (syntax) /$unstock {database_id} {category} or $unstock {database_id} {category}

.. default:
Default
----------------

Default commands available to every user:

- **gen command** | receive a random item from the database

.. code-block:: console

   (syntax) /gen {category} or $gen {category}
   
- **ping command** | shows the input delay

.. code-block:: console

   (syntax) /ping or `$ping`

- **stock command** | prints all categories and their items number

.. code-block:: console

   (syntax) /stock or $stock

- **docs command** | the anchor to this docs site

.. code-block:: console

   (syntax) /docs or $docs



