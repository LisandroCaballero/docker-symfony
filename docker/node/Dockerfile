FROM node:12

# Update NPM
RUN npm install -g npm

# Set USER
RUN groupmod -g 999 node && usermod -u 999 -g 999 node
RUN useradd -ms /bin/bash project
USER project
WORKDIR /home/project/app

CMD tail -f /dev/null
