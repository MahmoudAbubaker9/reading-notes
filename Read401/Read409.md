# WRRC and Java

### The HTTP Request Lifecycle

Every Http request first contacts a DNS server which resolves the request URL domain to a IP address. After fetching the Webserver IP address request is forwarded to it(via PUT request).

**Step 1: Local Processing**

**Step 2: Resolve an IP**

**Step 3: Establish a TCP Connection**

**Step 4: Send an HTTP Request**

**Step 5: Tearing Down and Cleaning Up**

**explain**

1- in beginning the browser need to convert the (www.example.com) to an IP address.


2- Then browser will open a TCP connection to the IP address of (www.example.com) and send a HTTP GET request over.

3- The server software will get this HTTP request. It will generate a HTTP response and send that back trough the TCP connection.

4-When the browser gets the response, it typically renders it on screen. The HTTP request is now done.

For more Information --> [resource](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

### Java HTTP Request example

1. HttpUrlConnection :

is aclass allows us to perform basic HTTP requests without the use of any additional libraries , is part of the java.net package.

2. Creating a Request :

we can creates a connection object by create an HttpUrlConnection instance using the openConnection() method of the URL class

```
URL url = new URL("http://example.com");
HttpURLConnection con = (HttpURLConnection) url.openConnection();
con.setRequestMethod("GET");
```

4. Adding Request Parameters :

we have to set the doOutput property to true, then write a String of the form

5. Setting Request Headers : 

can be achieved by using the setRequestProperty() method

6. Configuring Timeouts :

Configuring Timeouts can allow us to setting the connect and read timeouts

7. Handling Cookies :

The java.net package contains classes that ease working with cookies

8. Handling Redirects : 

when it is encoded into a web page rather then set on a server level

There are five types of redirects: 301, 302, 303, 307, and 308

9. Reading the Response

10. Reading the Response on Failed Requests

11. Building the Full Response

For more Information --> [resource](https://www.baeldung.com/java-http-request)
