Here is the process i used for my basic microservice application using Kubernetes
The first step was to build the services i would need.
User service flask ( python file,requirement.txt,dockerfile)
Order service flask (python file,requirement.txt,dockerfile)
Frontend (python file,requirement.txt,dockerfile)
I then made docker images of the corresponding files
Then i pushed the images from docker to kubernetes
Next i created manifest of the user service,order service and frontend
I used the kubeclt -f apply (file) command on each file to create the pods
I then port forwarded the internal ip address so i would be able to reach it externally.
Project was a success. I was able access the web application.
