Part 1
---

A web server called StringServer that supports the path and behavior is described below. It keeps track of a single string that gets added to by incoming requests.     


```

import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    StringBuilder StrBui = new StringBuilder();

    public String handleRequest(URI url) {
        if (url.getPath().contains("/add-message")) {
            StrBui.append(url.getQuery().substring(2)+"\n");
            return StrBui.toString();
        } else {
            System.out.println("Path: " + url.getPath());
            return "404 Not Found!";
        }
    }
}
class NumberServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
The code generates this when run:

<img width="600" alt="image" src="https://user-images.githubusercontent.com/130006438/233950869-ea2d0ed7-43b2-4950-9af9-1193897533f1.png">


The StringServer class's main method instantiates a new Handler object to process incoming requests. The Handler class provides the handleRequest method, which parses request paths and query parameters to create a response for display on a web page. If a request path contains "/add-message?s=", the value of the "s" parameter is extracted and appended to the str instance variable. str is a StringBuilder object that stores all the passed strings, with each new string added on a new line every time the page loads. If the request path does not include "/add-message?s=", the server returns a "404 Not Found" error, indicating that the requested resource cannot be found. This behavior is because handleRequest is programmed to only process requests that have the "s" parameter. If the "s" parameter is present, the server prints the contents of the str instance variable.

`/add-message?s=hi  `       prints this on the webpage

<img width="600" alt="image" src="https://user-images.githubusercontent.com/130006438/233951095-d468188e-a100-4eaa-8b2a-2790347eb202.png">
<img width="600" alt="image" src="https://user-images.githubusercontent.com/130006438/233958338-1bcc3c2a-3984-49dc-b068-017ea2202270.png">

This code has two classes(Handler and NumberServer).


Part 2
---

  The 'reversed' method sets the values of the new array to the old one instead of the other way. So, it does not reverse the array as values are not replaced. The array in the parameter was replaced by the values in the new Array. This made it blank.
  
  So, it can only have values that are zero.

  The test below is a non failure inducing input for the method.
` 
@Test
public void testReversed () {
int [] input1 = { };
assertArrayEquals(new int [l{ }, ArrayExamples.`
  

  The test below is failed by this method.
 
 <img width="405" alt="image" src="https://user-images.githubusercontent.com/130006438/233964297-3d1fcb9f-fd9d-48ed-8930-2fd53bd78284.png">
A screenshot of the output was:
<img width="968" alt="image" src="https://user-images.githubusercontent.com/130006438/236777799-d0421108-f832-4b59-9823-61e8651b90bd.png">

**Code before:**
  ```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
  ```
  **Code after:**
  ```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
 ```
 Basically, what this code does is that it places te values in the newArray in reverse order from the array(arr) that is input as the parameter.
 Earlier, the array in the parameter was replaced by the values in the new Array. This made it blank.
---
Part 3
---
These two weeks mainly helped me understand where this course was heading forward too. More specifically, I learned about finding bugs by going through code, and other specific commands. 
