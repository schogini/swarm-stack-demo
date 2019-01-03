# Use an official Python runtime as a parent image
FROM python:2.7-slim


WORKDIR /app
ADD . /app
RUN pip install --trusted-host pypi.python.org Flask Redis
# RUN pip install --trusted-host pypi.python.org -r requirements.txt
EXPOSE 80
ENV NAME World
CMD ["python", "app.py"]

# docker build -t schogini/vote-app:p80 docker-compose/app
# docker push schogini/vote-app:p80
# run -d -p 8080:80 --rm --name temp --network puppet temp
# docker run -d --rm --name redis --network puppet redis:alpine
# curl localhost:8080
# <h3>Hello World!</h3><b>Hostname:</b> b3f2f3a731a6<br/><b>Visits:</b> 1