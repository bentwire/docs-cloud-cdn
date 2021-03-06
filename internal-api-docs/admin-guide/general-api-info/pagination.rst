.. _pagination:

Pagination
~~~~~~~~~~

Pagination provides the ability to limit the size of the returned data
in the response body and to retrieve a specified subset of a large data
set. Pagination has two key concepts: *limit* and *marker*.

-  ``limit`` is the restriction on the maximum number of items that can
   be returned.

-  ``marker`` is the last item in the previous list returned.

   For example, a query could request the next 10 services after the
   service ``xyz`` as follows: ``?limit=10&marker=xyz``.

Pagination applies only to operations listed in the following operation:

+---------+---------------------------------------------+--------------------------------------------+
|  Verb   |                     URI                     |                Description                 |
+=========+=============================================+============================================+
| **GET** | /v1.0/services                              | Retrieves a list of all services.          |
+---------+---------------------------------------------+--------------------------------------------+

For an example, see the "Retrieve all services" operation description in the API operations section.