FROM ubuntu:20.04

# Install wget,Powershell
RUN apt-get update 
RUN apt-get install -y wget apt-transport-https software-properties-common     
RUN wget -q https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb
RUN dpkg -i packages-microsoft-prod.deb 
RUN apt-get update 
RUN add-apt-repository universe 
RUN apt-get install -y powershell 

#install curl, Node.js 16 and npm 8
RUN apt-get update -y
RUN apt install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt-get -y update
RUN apt-get install -y nodejs
RUN curl -L https://www.npmjs.com/install.sh | sh

RUN npm install sfdx-cli --global 
RUN npm install @salesforce/cli --global 

#install python 3.9
RUN apt-get update 
RUN add-apt-repository ppa:deadsnakes/ppa 
RUN apt-get install -y python3.9 

    




