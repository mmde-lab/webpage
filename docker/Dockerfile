FROM python:3.8.2
ENV PYTHONUNBUFFERED 1

# Install mkldocs etc...
WORKDIR /root
ADD requirements.txt /root/
RUN pip install --upgrade pip
RUN pip3 install -r /root/requirements.txt

VOLUME /root/mmde-lab-official-web
WORKDIR /root/mmde-lab-official-web
