Order
=====

This resource can be accessed via following URLs.

   * http://test.com/starbucks/{orderId}

deleteOrder (DELETE)
--------------------

   Remove the order identified by the specified ID from the system

   **Response Type**: :doc:`data_type_order`

   **Supported Response Media Types**: 
      * application/json

   **Sample Response**:: 

      {
          "orderId": "string",
          "additions": [
              "string1",
              "string2",
              "string3"
          ],
          "drink": "string",
          "cost": 12.345,
          "next": "http://example.com"
      }

   **Return HTTP Status**: 200 OK

   **Errors**:
      * 500 Internal Server Error - An unexpected runtime exception
      * 404 Not Found - Specified order does not exist

   **Example Curl Command**::

      curl -v -X DELETE http://test.com/starbucks/{orderId}

getOrder (GET)
--------------

   Retrieve the order identified by the specified identifier

   **Response Type**: :doc:`data_type_order`

   **Supported Response Media Types**: 
      * application/json

   **Sample Response**:: 

      {
          "orderId": "string",
          "additions": [
              "string1",
              "string2",
              "string3"
          ],
          "drink": "string",
          "cost": 12.345,
          "next": "http://example.com"
      }

   **Return HTTP Status**: 200 OK

   **Errors**:
      * 500 Internal Server Error - An unexpected runtime exception
      * 404 Not Found - Specified order does not exist

   **Example Curl Command**::

      curl -v http://test.com/starbucks/{orderId}

