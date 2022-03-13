# Read: 09 - WRRC and Java

## HttpUrlConnection

The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries.    
The disadvantages of using this method are that the code can be more cumbersome than other HTTP libraries and that it does not provide more advanced functionalities such as dedicated methods for adding headers or authentication.   
## Creating a Request  
We can create an HttpUrlConnection instance using the openConnection() method of the URL class.   
The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE.   
## Adding Request Parameters   
If we want to add parameters to a request, we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance:   
To facilitate the transformation of the parameter Map, we have written a utility class called ParameterStringBuilder containing a static method, getParamsString(), that transforms a Map into a String of the required format:   
## Setting Request Headers   
Adding headers to a request can be achieved by using the setRequestProperty() method:    

con.setRequestProperty("Content-Type", "application/json");       
To read the value of a header from a connection, we can use the getHeaderField() method:       

String contentType = con.getHeaderField("Content-Type");     
 
## Configuring Timeouts   
 These values define the interval of time to wait for the connection to the server to be established or data to be available for reading.    

To set the timeout values, we can use the setConnectTimeout() and setReadTimeout() methods:    

con.setConnectTimeout(5000);   
con.setReadTimeout(5000);   

## Handling Cookies   
The java.net package contains classes that ease working with cookies such as CookieManager and HttpCookie.  

First, to read the cookies from a response, we can retrieve the value of the Set-Cookie header and parse it to a list of HttpCookie objects:   

String cookiesHeader = con.getHeaderField("Set-Cookie");    
List<HttpCookie> cookies = HttpCookie.parse(cookiesHeader);   
Next, we will add the cookies to the cookie store:    

cookies.forEach(cookie -> cookieManager.getCookieStore().add(null, cookie));    
Let's check if a cookie called username is present, and if not, we will add it to the cookie store with a value of “john”:   

Optional<HttpCookie> usernameCookie = cookies.stream()    
  .findAny().filter(cookie -> cookie.getName().equals("username"));   
if (usernameCookie == null) {    
    cookieManager.getCookieStore().add(null, new HttpCookie("username", "john"));   
}   
Finally, to add the cookies to the request, we need to set the Cookie header, after closing and reopening the connection:    

con.disconnect();   
con = (HttpURLConnection) url.openConnection();    

con.setRequestProperty("Cookie",    
  StringUtils.join(cookieManager.getCookieStore().getCookies(), ";"));   
  
## Reading the Response   
Reading the response of the request can be done by parsing the InputStream of the HttpUrlConnection instance.    

To execute the request, we can use the getResponseCode(), connect(), getInputStream() or getOutputStream() methods:    

int status = con.getResponseCode();    
  
To close the connection, we can use the disconnect() method:   

con.disconnect();   

## Reading the Response on Failed Requests   
If the request fails, trying to read the InputStream of the HttpUrlConnection instance won't work. Instead, we can consume the stream provided by HttpUrlConnection.getErrorStream().   
  
  
