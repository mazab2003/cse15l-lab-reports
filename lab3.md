
** Grep -r Command**

Example 1 :


<img width="1102" alt="Screen Shot 2023-02-13 at 11 27 02 PM" src="https://user-images.githubusercontent.com/110417533/218668097-4408be05-972c-4973-877d-365a30f9be44.png">



Example 2 : 


<img width="713" alt="Screen Shot 2023-02-13 at 11 25 10 PM" src="https://user-images.githubusercontent.com/110417533/218667757-6ce1d090-0cb8-4030-bed4-a65067b84987.png">


* grep -r is such a powerful command, as it searches through all the files in the directory and its subdirectories recursively. In the first example, it was used with -c to search for NYC and San Diego and indeed it returned all the lines that contained any of those words. In the second example I used the command alone to search for Los Angeles and all the occurunces of Los Angeles in the text got returned.*


** Grep -l Command**

Example 1 : 

<img width="636" alt="Screen Shot 2023-02-13 at 11 36 07 PM" src="https://user-images.githubusercontent.com/110417533/218670099-66d530f1-73fb-47ae-9cb4-88bfa6d41a94.png">


Example 2 : 

<img width="595" alt="Screen Shot 2023-02-13 at 11 36 44 PM" src="https://user-images.githubusercontent.com/110417533/218670117-3f1aeb5e-2400-49a6-b7c8-518bbf0f8ecb.png">

*grep -l prints the name of the files that matches the entered string, I combined the last command -r to search recursivly
through the files for Manhattan and Food and I got all the results.*

** Grep -c **

Example 1 ; 

<img width="588" alt="Screen Shot 2023-02-13 at 11 40 43 PM" src="https://user-images.githubusercontent.com/110417533/218671769-0deba26f-fc5f-4db5-ac91-96af136a41a2.png">


Example 2 : 

<img width="617" alt="Screen Shot 2023-02-13 at 11 45 56 PM" src="https://user-images.githubusercontent.com/110417533/218671845-1bd52832-69fa-4898-bea9-0b157ffbb2ad.png">

*This command prints the number of lines that matches the pattern. Here I searched for OpenAi and UCSD and every line that contains that pattern got returned*

** grep -w**

Example 1 :

<img width="700" alt="Screen Shot 2023-02-13 at 11 48 31 PM" src="https://user-images.githubusercontent.com/110417533/218672528-3cbc021b-a641-4aa6-b52b-6f4d3a4cafec.png">

Example 2 : 

<img width="692" alt="Screen Shot 2023-02-13 at 11 49 18 PM" src="https://user-images.githubusercontent.com/110417533/218672580-1338313d-c03a-4b2f-97e6-8c978ff5699c.png">

*I really liked this command, it searches for the whole word that matches the pattern. I searched for La Jolla and Wall Street in the exmaples and I got were 
exactly those words were mentioned.*

*I used ChatGPT as a resource to know more about the commands and to get examples*

