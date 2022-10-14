# Part 1 of Week3 Lab 

## Code 

import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String[] s = {};

    public String handleRequest(URI url)
          {  if (url.getPath().contains("/add")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("add?s")) {
                  
                    return String.format("added"
                    );
                }
                if (parameters[0].equals("search?s")){
                    return String.format("appSearch");
                }
            }
            return "404 Not Found!";
        }
    }


class SearchEngine{
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }
    }}

   


   ## Using URL
   ![Image](https://user-images.githubusercontent.com/114532765/195786193-f2d3e624-bcb3-422b-9e43-452b58c0805d.png)
   I understand that I must test out different paths and queries in my browser, but I could not successfully do this as I did in NumberServer. I typed in the commands for windows given in the lab into the terminal. Next, I opened another tab and tested out different URLs, but the site cannot be reached. 

   # Part Two 
   ## Failure Inducing Input 

    @Test 
  public void testReverseInPlace1(){
    int[] input4 = {4,5,6,7,8};
    int[] output = {8,7,6,5,4};
    ArrayExamples.reverseInPlace(input4);
    assertArrayEquals(output, input4);
   } 

 ## Symptom (output)
 {8,7,6,7,4}
 ## The Bug 
 static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {//4,5,6,7,8
      arr[i] = arr[arr.length - i - 1];
    }
  }
  
  Here, I changed the for loop to iterate through only half of the array length instead of full. The bug in the code is that after the first half of the elements in the new array is assigned, it continues to change the second half, which had already been changed. Once the for loop gets to the second half it will already have been changed, so the program cannot use the original numbers. In order to change this, the for loop needs to loop through half of the length.

## Second Test 
## Failure Inducing Input 
@Test

   public void TestReversal(){
    int [] input8 ={1,2,3,4,5};
    int[] output5 ={5,4,3,2,1};
    ArrayExamples.reversed(input8);
    assertArrayEquals(output5, input8);
   }

   ## Symptom 
   {1,2,3,4,5}

   ## Bug (fix)
     static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }

  The problem was that the code returned the original array instead of the new Array.To fix this bug, I switched the placement of newArray and arr and changed the program to return newArray. 





