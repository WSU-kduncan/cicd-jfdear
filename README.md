Project Overview -   
Containerize an application with Docker  
Automate the project pipeline with GitHub Actions  
Explore usage of webhooks to keep production up to date  
  
Run Project Locally  
how you installed docker + dependencies (WSL2, for example)  
I did this on my AWS instance  
I set up a repository by running the commands listed below  
![image](https://user-images.githubusercontent.com/77360294/144364432-bcb5ad71-16bd-4817-aab3-00f8ea4d97a9.png)  
I installed the engine using the commands below and docker was working  
![image](https://user-images.githubusercontent.com/77360294/144364512-fff8b1a5-7a14-434f-9ce4-2f0d68ed6040.png)  

Used the httpd dependency to help with running the container(please tell me if this is not supposed to go here)  

how to build the container  
sudo docker build -t project6:latest .  

how to run the container  
sudo docker run -dit -p 8080:80 project6  

how to view the project (open a browser...go to ip and port...)  
![how_to_view_project](https://user-images.githubusercontent.com/77360294/144363107-670c234f-25dd-4223-a9bb-0cea287e29e0.PNG)  
