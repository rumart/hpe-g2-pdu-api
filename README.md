# HPE G2 Metered and Switched PDU - REST API

The [HPE G2 PDUs](https://www.hpe.com/us/en/product-catalog/servers/power-distribution-units/pip.power-distribution-units.1009830118.html) ship with a REST API based on the Redfish standard. This is nice, but as of this writing the documentation for the API is completely missing.

## Postman collection

I've created a Postman collection for some (if not all) of the available endpoints. Please note that I've only added GET examples.

The collection shows examples on how to retrieve information about the different PDUs that are connected and also how to pull the utilization on the Load segments as well as the different outlets in each segment.

To learn how you can work with Postman collections check out the Intro to collection in the [Postman documentation](https://www.getpostman.com/docs/v6/postman/collections/intro_to_collections), and details on how to import collection can be found [here](https://www.getpostman.com/docs/v6/postman/collections/data_formats#exporting-and-importing-postman-data)

If you want to check out the endpoints feel free to download the Postman collection and start playing with it in your Postman client. 

__Authentication__

The examples are built with Basic Auth authentication. In the collection you need to update the Authorization tab with credentials that works in your environment

__Variables__

All examples requires a _mgmtIp_ variable where you specify the Management IP address.
To pull details about PDUs you will also need to include the PDU id in the _pduId_ variable, and for the segment utilization you need to specify the _segmentId_ variable.

To specify variables in your collection check out the [Postman documentation](https://www.getpostman.com/docs/v6/postman/environments_and_globals/variables#defining-collection-variables)