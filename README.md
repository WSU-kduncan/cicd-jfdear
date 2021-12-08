Part 1  
  
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

Used the httpd dependency to help with running the container  

how to build the container  
sudo docker build -t project6:latest .  

how to run the container  
sudo docker run -dit -p 8080:80 project6  

how to view the project (open a browser...go to ip and port...)  
![how_to_view_project](https://user-images.githubusercontent.com/77360294/144363107-670c234f-25dd-4223-a9bb-0cea287e29e0.PNG)  
  
Part 2  
  
Create DockerHub public repo  
![creating_repo](https://user-images.githubusercontent.com/77360294/145151852-c304c137-3371-4bb2-af74-8bb6dd2b60a4.PNG)  

Allow DockerHub authentication via CLI using Dockhub credentials  
![CLI_access](https://user-images.githubusercontent.com/77360294/145151918-9845df6b-a115-4558-939a-05a3387932fe.PNG)  

Configure GitHub Secrets  
What credentials are needed - DOCKER_USERNAME(GitHub username) and DOCKER_PASSWORD(the CLI token)  
set secrets and secret names  
![docker secrets](https://user-images.githubusercontent.com/77360294/145152066-2885341e-f67d-442c-9db5-9553a499b1b6.PNG)  

Configure GitHub Workflow  
variables to change (repository, etc.)  
![image](https://user-images.githubusercontent.com/77360294/145269567-46282d5c-eaf6-4f59-bab4-b1e671b8f5b6.png)  
  
Showing it worked  
![image](https://user-images.githubusercontent.com/77360294/145269701-08418e7e-1f5d-4b63-9950-78b6d8651900.png)  
![image](https://user-images.githubusercontent.com/77360294/145269768-fb4eadee-1b4c-4bfd-a2f5-e9ca15190e5d.png)  


