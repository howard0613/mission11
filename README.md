Hello!

This is my mission11 !!!
 
最最基本的jupyter notebook

  #docker-compose.yml:
    
version: '3'

services:
    datascience-notebook:
        image: jupyter/base-notebook:latest
        volumes:
            - /tmp/jupyter_test_dir:/home/docker_worker/work            
        ports:
            - 8891:8888
        command: start-notebook.sh --NotebookApp.token=''
