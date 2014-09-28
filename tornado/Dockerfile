FROM debian
RUN yes | apt-get update -q
RUN yes | apt-get install curl python3-dev && curl -sL https://raw.github.com/7t/dockerfiles/master/tornado/get-pip.py | python3
ADD . /home/tornado
RUN pip install -r requirements.txt
