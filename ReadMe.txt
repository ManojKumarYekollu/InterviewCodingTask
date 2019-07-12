1. For getting all the available vending machines
URL				: http://localhost:8080		
Request Type	: GET

2. For getting Single Machine 
URL				: http://localhost:8080/{MachineId}
Example 		: http://localhost:8080/2	 
Request Type	: GET

3. For Adding a new Machine 
URL				: http://localhost:8080
Example 		: http://localhost:8080	 
Request Type	: POST
Request Body(JSON) 	: 
{
	
	"name": "MachineThree",
    "currentAmount": 2000
}


4. For getting a products in a machine
URL				: http://localhost:8080/{MachineId}/products
Example 		: http://localhost:8080/3/products
Request Type	: GET

5. For Adding a product in to the machine
URL					: http://localhost:8080/{MachineId}/products
Example 			: http://localhost:8080/3/products
Request Type		: POST
Request Body(JSON) 	:  
{	
	"name": "7up",
	"cost": 120,
	"quantity": 5
}

6. For Purchasing a Product
URL					: http://localhost:8080/{MachineId}/products/{productId}/buy
Example 			: http://localhost:8080/3/products/7/buy
Request Type		: GET

7. Getting a particular product
URL					: http://localhost:8080/{MachineId}/products/{productId}
Example 			: http://localhost:8080/3/products/7
Request Type		: GET

8. Getting a no.of coins in machine product
URL					: http://localhost:8080/{MachineId}/coins
Example 			: http://localhost:8080/3/coins
Request Type		: GET

9. Adding a coin in to the machine
URL					: http://localhost:8080/{MachineId}/coins
Example 			: http://localhost:8080/3/coins
Request Type		: POST
Request Body(JSON) 	:  
 {
        "id": 5,
        "value": 50,
        "amount": 5
 }
 
10. Get all the money that has not been spent in the system 
URL						: http://localhost:8080/{MachineId}/coins/unused
Example 				: http://localhost:8080/3/coins/unused
Request Type			: GET

11. Get the coin information on a machine
URL						: http://localhost:8080/{MachineId}/coins/{coinvalue}
Example 				: http://localhost:8080/3/coins/50
Request Type			: GET


 

