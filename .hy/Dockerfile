FROM ubuntu
RUN apt-get update --fix-missing && apt-get -y install python3.6 && apt-get clean
RUN apt-get update --fix-missing && apt-get -y install python3-tk && apt-get clean
RUN apt-get update --fix-missing && apt-get -y install python3-pip && apt-get clean
RUN pip3 install grpcio
RUN mkdir /wall && cd /wall && apt-get update --fix-missing && apt-get -y install git && apt-get clean && git clone --branch wall https://github.com/josemibnf/SAT-Wall.git && mv SAT-Wall/* . && rm -rf SAT-Wall && rm -rf .git
