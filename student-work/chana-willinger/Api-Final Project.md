## GET/tableNo

This is the call that is sent when the server wants to get the bill the GET request includes the table number. The order number is included in the response.Take out orders are table 99. When this is printed, the customer can pay the bill.

GET request

curl -X GET "http://URL/tableNo?id=99"

Response:

![image](https://user-images.githubusercontent.com/98663506/179369750-4111067f-2ab1-4645-89d7-69d9c4e29f77.png)


The following are the items include the information in the order.

| orderNum     | int     | The order number               
|--------------|---------|-------------------------------
| timestamp    | int     | The time the order was placed  
| Item1        | string  | Describes the order placed     
| ItemOrdered  | string  | Describes the type of meal     
| type         | string  | Food type                      
| cost         | int     | Cost of food item              
| Item2        | string  | Second food order placed       

