# CS361_MainProgram
Repository  for my Microservice A for CS361

Communication contract: We will use zmq for communication. 

A. You can request news articles for a user by sending a json file containing the list of favorite stocks for that user:
    example call: favorite_stocks = ["vti", "nvda", "goog", "cost"]
                  socket.send_json(favorite_stocks)

B. When the Microservice is finsihed running it will have created a new json file that it will return:
    example call: news_list = socket.recv_json()

    (docs/UML_MicroserviceA.png)
    
                  
    
