# spark-streaming
Getting started with spark streaming

"""
 Counts words in UTF8 encoded, '\n' delimited text received from the network every second.
 Usage: python network_wordcount.py <hostname> <port>
   <hostname> and <port> describe the TCP server that Spark Streaming would connect to receive data.
 To run this on your local machine, you need to first run a Netcat server
    `$ nc -lk 9999`
 and then run the example
    `$ python network_wordcount.py localhost 9999`
"""