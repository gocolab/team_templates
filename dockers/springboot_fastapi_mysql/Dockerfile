FROM python:3.11

# install any packages
RUN apt-get update && \
    apt-get install -y openjdk-17-jdk fonts-nanum wget unzip

# setup JAVA_HOME configuration
ENV JAVA_HOME /usr/lib/jvm/java-17-openjdk-amd64

# setup fastapi
WORKDIR /apps

ARG APP_DIR_NAME_FASTAPI

# Clone the Git repository. Here we dynamically specify the repository name using the variable defined earlier.
RUN git clone -b data_engineers https://github.com/gocolab/co_templates ${APP_DIR_NAME_FASTAPI}

# Changes the working directory to /apps/${REPO_NAME}. This uses the variable to dynamically set the directory path.
WORKDIR /apps/${APP_DIR_NAME_FASTAPI}/app

RUN pip install --no-cache-dir -r ./requirements.txt

WORKDIR /apps/${APP_DIR_NAME_FASTAPI}

# RUN rm -rf .git

# setup springboots
WORKDIR /apps

ARG APP_DIR_NAME_SPRINGBOOT

# Clone the Git repository. Here we dynamically specify the repository name using the variable defined earlier.
RUN git clone -b main https://github.com/yojulab/learn_springboot3_gradle_security ${APP_DIR_NAME_SPRINGBOOT}

# Changes the working directory to /app/${REPO_NAME}. This uses the variable to dynamically set the directory path.
WORKDIR /apps/${APP_DIR_NAME_SPRINGBOOT}

# RUN rm -rf .git
