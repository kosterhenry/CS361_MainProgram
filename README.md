# CS361_MainProgram
Repository  for my Microservice A for CS361

Communication contract: We will use zmq for communication. 

A. You can request news articles for a user by sending a json file containing the list of favorite stocks for that user:
    example call: favorite_stocks = ["vti", "nvda", "goog", "cost"]
                  socket.send_json(favorite_stocks)

B. When the Microservice is finished running it will have created a new json file containing 5 most recent news articles on each favorited stock
    the articles will each contain the info (title, url, source, date):
    example call: news_list = socket.recv_json()

![image alt](https://raw.githubusercontent.com/kosterhenry/CS361_MainProgram/main/UML_MicroserviceA.png)
