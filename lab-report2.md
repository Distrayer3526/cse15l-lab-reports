# Part 1
```Java
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String stringList = "";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return stringList;
        } 
        else if (url.getPath().equals("/add-message")) {
            String[] parameters = url.getQuery().split("=");
            if (parameters[0].equals("s")){
                stringList = stringList + "\n" + parameters[1];
            }
        }
        else{
            return "Invalid input. Try /add-message?s=[something_to_add]";
        }
        return stringList;
    }
}


class StringServer {
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
![image](https://user-images.githubusercontent.com/62564887/215288349-12c8e11a-3438-4ad9-9d46-bd0c1bae37e8.png)
* Since the server was already up and running, this input would only call the `handleRequest` method. Then to read in the url it uses the `getPath()` and `getQuery()` methods that are defined for URI data types. It also uses the `equals()` method from the Object interface. 
* This method needs a URI data type which get read by the other helper methods such as `getPath()` and `getQuery()`. Then there is also the string which holds all the user input. Intially the string is empty and the URI is just `localhost:4000/`.
* After running this specific request, the URI becomes `localhost:4000/add-message?s=dog`. The string list parameters gets defined and holds `[s, dog]`. And finally the empty `stringList` variable gets defined to hold `"dog"`. 

![image](https://user-images.githubusercontent.com/62564887/215288805-089c767c-ba56-4f04-a3c6-7997f534f629.png)
* This time the `handleRequest`, `getPath()`, and `equals()` methods will be called. `getQuery()` won't be called because this request will not even enter the loop which has that method call. `getPath()` and `equals()` will only be called because the if statement check for them
* Again, `handleRequest` needs a URI and the other methods need to the URI to be defined.
* The URI that gets made will change since it will have a value to `localhost:4000/something-else`. However the `stringList` variable won't change since the correct URI was not given and the string list parameters won't get defined this time. The return value will also be different since it tries to get the user to put in a correct value. 

# Part 2
I am going to talk about the reversed method in ArrayExamples
1. A failure-inducing input for the program
```Java
    int[] input2 = {1,2,3,4};
    assertArrayEquals(new int[]{4,3,2,1}, ArrayExamples.reversed(input2));
```
2. A non-failure-inducing input for the program
```Java
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
```
3. ![image](https://user-images.githubusercontent.com/62564887/215289625-624e5075-9ea7-4de2-9412-4035129097bc.png)
4. Before and after code
  * Before
```Java
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
  * After
```Java
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
5. In the buggy code, the original array with the actual values was being overriten by the new array that had just been created and was therefore empty. Basically all the value replaced by a 0. In the fixed code, we reversed the array calls so that the new empty array was filled with values from the original array but in the reverse order. 

# Part 3
In the lab in week 2 I learned how to make a private and remote access webpage. I learned about a new data type called URI and how that can be used to achieve this. I learned about the different parts of a URL such the query and the path and how I could access those with code and change how my webpage works. In week 3 I didn't learn anything new per se but I did see hwo thoroughly code should be tested and how JUnit it one of those tools that can make life a lot easier for that. I saw that bugs are not always readily apparent and that thorough testing it required to sometimes find a minor bug. Code should be run through every loops that exists in a method to completely check if everything works properly. However, I also know its impossible to check every single thing that could go wrong in a program but it is our job to mitigate the amount of errors that could occur. 
