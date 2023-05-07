# qa tool sharing exercise

Please use java 11+ for project setup.

Common use cases:

1. Get access token by calling http get on http://localhost:8080/users/token?login=login1&password=pass1
2. Get all accessible phones by calling hhtp get on http://localhost:8080/phones?token=QWERTY12323434JJJJ 
    with body example:
    {
        "page": 0,
        "perPage":20,
        "available":true,
        "label":"AIP_13_1",
        "bookerNickName":"jonny"
    }
3. Try to book some device :

    http://localhost:8080/phones/6?token=QWERTY12323434JJJJ&toBook=true
    
    here you could try to book device with id 6.
    
4. Get rich information from external system:
   
   http://localhost:8080/phones/full/6?token=QWERTY12323434JJJJ
   
   here you will get full information with data from third-party service
