Part 1
---

code: 

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
<img width="447" alt="image" src="https://user-images.githubusercontent.com/130006438/233950869-ea2d0ed7-43b2-4950-9af9-1193897533f1.png">
<img width="447" alt="image" src="https://user-images.githubusercontent.com/130006438/233951095-d468188e-a100-4eaa-8b2a-2790347eb202.png">
<img width="447" alt="image" src="https://user-images.githubusercontent.com/130006438/233958338-1bcc3c2a-3984-49dc-b068-017ea2202270.png">

This code has two classes(Handler and NumberServer).
---
---

Part 2
---

  It sets the values of the new array to the old one instead of the other way.
  
  So, it can only have values that are zero.
  The test below is passed by the method.
<img width="529" alt="image" src="https://user-images.githubusercontent.com/130006438/233964912-4194b8f5-e848-4321-abb3-d3ddf73cc6c1.png">
  

  The test below is failed by this method.
 
 <img width="405" alt="image" src="https://user-images.githubusercontent.com/130006438/233964297-3d1fcb9f-fd9d-48ed-8930-2fd53bd78284.png">

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
---
Part 3
---
These two weeks mainly helped me understand where this course was heading forward too. More specifically, I learned about finding bugs by going through code, and other specific commands. 
