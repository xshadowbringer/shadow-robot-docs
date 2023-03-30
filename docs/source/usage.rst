Commands
=====

.. _installation:

Administrator
------------

- Addstock command

.. code-block:: console

   (syntax) /addstock

-  config

.. code-block:: console

   (syntax) /config or $config
   >>> setup
   if you database limit is not reached you will have to follow 4 steps :
               1. Enter channels ID's that receiving an item is allowed
               2. Enter roles ID's that are allowed to see the current stock of the item
               3. Enter channels ID's that seeing the current items stock is allowed
               4. Enter the channel ID of the log channel, that will print the receivings
           

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

