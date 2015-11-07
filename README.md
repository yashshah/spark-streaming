# spark-streaming
Getting started with spark streaming


## Installing Maven
Download Binary from [here](https://maven.apache.org/download.cgi). Extract it. Edit your bash_profile with this:

```
export M2_HOME=/Users/Yash/Downloads/apache-maven-3.1.1
export PATH=$PATH:$M2_HOME/bin
```

and run the following command to see if it has been properly installed or not:

```
$ mvm -v
```

I followed this manual installation of this [blog post](http://www.mkyong.com/maven/install-maven-on-mac-osx/).

## Installing Spark

Just go through all the steps mentioned in [this blog post](https://shellzero.wordpress.com/2015/07/24/how-to-install-apache-spark-on-mac-os-x-yosemite/)



## Running the Network count
It Counts words in UTF8 encoded, '\n' delimited text received from the network every second.

To run this on your local machine, you need to first run a Netcat server

```
$ nc -lk 9999
```

And then run the example inside the spark installation directory, run the following command:
```
$ ./bin/spark-submit <path_to_python_network_count_file> localhost 9999

```