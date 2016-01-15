FROM node
MAINTAINER Basil Veerman <bveerman@uvic.ca>

RUN git clone https://github.com/seejohnrun/haste-server.git /opt/haste
WORKDIR /opt/haste
RUN npm install

ADD config.js /opt/haste/config.js

EXPOSE 7777

CMD ["npm", "start"]