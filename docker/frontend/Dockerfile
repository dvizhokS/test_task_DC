FROM node:21

RUN apt-get update && apt-get install -y zip unzip

WORKDIR /var/www/

#CMD ["tail", "-f", "/dev/null"]
CMD ["npm", "run", "dev", "--", "--host"]
