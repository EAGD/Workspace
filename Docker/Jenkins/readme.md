# Docker commands to run
- docker build -t <containerName> . <br>
- docker run -p 8080:8080 -p 50000:50000 <containerName> <br>

# Docker commands
- docker -v <br>
- docker ps -a <br>
- docker stop <containerId> <br>
- docker rm <containerId> <br>

# Git commands
- git clone https://www.github.com/tu-repositorio-aqui <br>
- git config --global user.email "tu-correo" <br>
- git config --global user.name "tu-nombre" <br>
- git add . <br>
- git commit -m "mensaje del commit" <br>
- git push origin main <br>

# Requirements to start
- docker
- git
- a public repository
# Guide to run and install this project

- Clone this repo and enter to the folder where your dockerfile is, then run the first command <br>
    "docker build -t jenkins ." yes, it's a point as last character, include it!<br>
- wait for the download of Jenkins image and the run the next command <br>
    "docker run -p 8080:8080 -p 50000:50000 jenkins <br>
- why two ports? because one is for the UI of jenkins (8080) and the 2nd is for the agent to execute the pipelines (50000) <br>
- once you execute the command, logs will appear in the console, then you have to open your browser and write <br>
    "localhost:8080/" <br>
- Jenkins will start and you have to write the admin password that would be available in the logs of your terminal, after that, please select the standard plugins and wait for the installation, if a plugin fail, wait for the others and re install the failed plugins <br>
- After the installation is completed, you can set a different user from the admin profile, if you don't want to create a new one, skip and click next as admin <br>
- Once you are in the initial or root dashboard of jenkins, look at the left menu and select the credentials option, select the jenkins credentials, then the global credentials and fill the information with your own github account to create specific credentials for your account and own repositories <br>

- Congrats, you have a functional CICD tool working now with credentials to interact with your own repository
- PD: make sure your repository is public and available
