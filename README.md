# pickmeup-db

Install Docker in Windows
Step1: Install 'docker tool box' in your laptop
        https://docs.docker.com/toolbox/toolbox_install_windows/

Step 1: Create docker machine
docker-machine create --driver virtualbox default

Step2: Check docker machine config
docker-machine env default

Step3: Configure shell
docker-machine env default | Invoke-Expression

Install Docker in Mac:
https://docs.docker.com/engine/installation/mac/


Build Docker Image(DB):
docker build -t pickmeup-db .

Build Docker Compose:
docker-compose build

Run Database Image:
docker-compose up -d pickmeup-db

Check logs for database image/container:
docker-compose logs -f pickmeup-db

Stop container(or DB):
docker-compose stop pickmeup-db
