<div align="center">

# 🪞 Mission Reflection

</div>

---

This laboratory activity gave me a better understanding of how Docker containers work and why they are useful in cloud computing. Before doing this activity, I had only a basic idea about containers, but using Docker to deploy an Nginx web server helped me understand the concept more clearly. Compared with a Virtual Machine, a Docker container can start much faster because it does not need to install or boot a complete operating system. Instead, it uses the host operating system and only runs the application and the resources it needs. This makes the setup process simpler and more efficient.

I also learned why port mapping is important when running a web server inside a container. The Nginx server runs on port 80 inside the container, but I used port 8080 on the host to access it. The `-p 8080:80` command connects these two ports, allowing me to open the Nginx server through `http://localhost:8080`. Without the port mapping, accessing the web server from the host would not work in the same way.

Another thing I learned was what happens when a container is removed using `docker rm`. The container and its writable data are removed, but the Docker image remains. Data stored separately in persistent volumes can also remain. This showed me why important data should be stored separately when using containers.

I think containerization can also improve teamwork between developers and IT operations because applications can be packaged with their required dependencies and run more consistently in different environments. Finally, my GitHub portfolio is slowly becoming more organized as I add each laboratory activity. It gives me a place to document what I have learned and provides evidence of the practical cloud computing skills I am developing.

---

