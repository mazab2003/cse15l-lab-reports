#Part 1

<img width="620" alt="Screen Shot 2023-02-12 at 11 40 42 PM" src="https://user-images.githubusercontent.com/110417533/218398947-307964c9-87c0-4348-bf3d-0d0284a8951e.png">


<img width="718" alt="Screen Shot 2023-02-12 at 11 40 19 PM" src="https://user-images.githubusercontent.com/110417533/218398961-d8af02bd-2c06-4101-bd4e-e31277504414.png">


<img width="743" alt="Screen Shot 2023-02-12 at 11 40 01 PM" src="https://user-images.githubusercontent.com/110417533/218398978-25de78fb-cd20-49ae-b7be-3a2e02bb26fb.png">

*I used ChatGPT to help with debugging the handleRequest method as I was having weird outputs such as printing the same work more than once
I also used some of the code provided in one of the labs to help with the server.*

*The first thing being called is the main method, which is calling ServerHandler to start the server. Inside ServerHandler both handle and start method are called. After that the StringServer code gets run.*

*The relevant argumetns are the port number and the handler in the start method. And the url in handleRequest*

*The port number changes depending on the port number entered in the command line, also toAdd, mylist, lab2, all gets changed depending on the string entered in the url path after the "="*

#Part2

<img width="468" alt="Screen Shot 2023-02-13 at 12 51 50 AM" src="https://user-images.githubusercontent.com/110417533/218412834-7cc3bb27-f73c-45e8-8972-ec2cbdebf2c2.png">

`public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
`
<img width="639" alt="Screen Shot 2023-02-13 at 12 52 48 AM" src="https://user-images.githubusercontent.com/110417533/218413011-da92ce24-60b7-44e6-8e01-d90808fc9283.png">

`public void testReverseInPlace2() {
    int[] testArr = {1,2,3};
    ArrayExamples.reverseInPlace(testArr);
    assertArrayEquals(new int[]{3,2,1}, testArr);
  }
`

<img width="680" alt="Screen Shot 2023-02-13 at 12 56 18 AM" src="https://user-images.githubusercontent.com/110417533/218413797-6ef48122-8936-451d-8ac5-e1d2af061fa1.png">

*Before*
`static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }`


*After* 
`static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int forRev = arr[arr.length-i-1];
      arr[arr.length-i-1] = arr[i];
      arr[i] = forRev;
    }
  }`
  
*The method before had two main issues that got fixed in the second code. Firstly, the for loop
was going through the whole array which is not necassary and do not work with that implementation.
Second issue that there was no temporary value that hold the old value before it get switched and 
both of the issues were fixed in the second code.*


#Part3

*I had no idea how to run a server, and I learned a lot of things about building and running servers 
on my local deivce and also remotely. Also my debugging skills improved from working on bugs on week 3, also 
I learned a lot of new vocabulary thats related to debugging.*
