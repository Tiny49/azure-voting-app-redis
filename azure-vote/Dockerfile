FROM tiangolo/uwsgi-nginx-flask:python3.6
RUN pip install redis
ADD /azure-vote /app

FROM jenkins
USER root
RUN apt-get update && apt-get install -y python-pip && rm -rf /var/lib/apt/lists/*