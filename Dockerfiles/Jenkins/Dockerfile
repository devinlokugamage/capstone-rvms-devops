FROM lokugamage186/jenkins-rvms:1.3
USER root

RUN apt-get install wget
RUN apt-get update && apt-get install unzip 
RUN wget  https://releases.hashicorp.com/packer/1.3.2/packer_1.3.2_linux_amd64.zip
RUN unzip packer_1.3.2_linux_amd64.zip -d packer
RUN mv packer /usr/local/
ENV PATH=$PATH:/usr/local/packer/

RUN packer --version
RUN java --version
RUN mvn --version
RUN docker --version
