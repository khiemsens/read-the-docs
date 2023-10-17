AllOrders
=========

This resource can be accessed via following URLs.

   * http://test.com/starbucks/

getAllOrders (GET)
------------------

   No description available

   **Response Type**: list(:doc:`data_type_order`)

   **Supported Response Media Types**: 
      * json

   **Return HTTP Status**: 200 OK

   **Example Curl Command**::

      curl -v http://test.com/starbucks

submitOrder (POST)
------------------

   No description available

   **Request Type**: :doc:`data_type_allorders_submitorder_inputtype`

   **Supported Request Media Types**: 
      * json

   **Response Type**: :doc:`data_type_order`

   **Supported Response Media Types**: 
      * json

   **Return HTTP Status**: 201 Created

   **Example Curl Command**::

      curl -v -X POST -d @input.txt -H "Content-type: json" http://test.com/starbucks

