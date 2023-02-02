
int num = 0;
    ArrayList<String> list = new ArrayList<>();
    ArrayList<String> myList = new ArrayList<>();
    StringBuilder Lab2 = new StringBuilder();
    public String handleRequest(URI url) {
        System.out.println("Path :" + url.getPath());
        if (url.getPath().contains("/add-message" )) {
            String[] toAdd0 = url.getQuery().split("=");
            String[] toAdd = url.getQuery().split("=");
            if (toAdd.length >= 2) {
                myList.add(toAdd[1]);
                Lab2.append(toAdd[1]).append("\n");
            }
            return Lab2.toString();

        }
  
  <img width="135" alt="Screen Shot 2023-02-01 at 4 52 23 PM" src="https://user-images.githubusercontent.com/110417533/216204163-1ee990a2-2edb-4f08-a7aa-cf50878f7022.png">
  
<img width="527" alt="Screen Shot 2023-02-01 at 4 51 47 PM" src="https://user-images.githubusercontent.com/110417533/216204179-61d2c5be-e37a-4e11-a4b0-90c969e94cd6.png">
  
  The method being called is handle request
  
  
  In the last two weeks : 
  I learned a better approach on how to debug programs, I also learned how to test the code using Junit
