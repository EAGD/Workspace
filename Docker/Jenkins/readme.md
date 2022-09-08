# Docker commands to run <br>
-docker build -t <containerName> . <br>
-docker run -p 8080:8080 -p 50000:50000 <containerName> <br>

# Docker commands in case of
-docker -v <br>
-docker ps -a <br>
-docker stop <containerId> <br>
-docker rm <containerId> <br>

# Git commands in case of <br>
-git clone https://www.github.com/tu-repositorio-aqui <br>
-git config --global user.email "tu-correo" <br>
-git config --global user.name "tu-nombre" <br>
-git add . <br>
-git commit -m "mensaje del commit" <br>
-git push origin main <br>


# Guide to run this project

-start entering inside the folder or where your dockerfile is, then run the first command <br>
    "docker build -t jenkins . <br>
-wait for the download of Jenkins image and the run the next command <br>
    "docker run -p 8080:8080 -p 50000:50000 jenkins <br>
-why two ports? because one is for the UI of jenkins (8080) and the 2nd is for the agent to execute the pipelines (50000) <br>
-once you execute the command, logs will appear in the console, then you have to open your browser and write <br>
    "localhost:8080/" <br>
-Jenkins will start and you have to write the admin password that would be available in the logs of your terminal, after that, please select the standard plugins and wait for the installation, if a plugin fail, wait for the others and re install the failed plugins <br>
- testing
