FROM python:3.12.7-slim-bookworm

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

WORKDIR /var/wow
COPY requirements.txt .
RUN pip3 install -r requirements.txt

ENTRYPOINT ["python3", "main.py", "-l", "world"]
