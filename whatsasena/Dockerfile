FROM fusuf/whatsasena:latest

RUN git clone https://github.com/phaticusthiccy/WhatsAsenaDuplicated /root/WhatsAsenaDuplicated
WORKDIR /root/WhatsAsenaDuplicated/
ENV TZ=Europe/Istanbul
RUN npm install supervisor -g
RUN yarn install --no-audit
RUN apk add python3
RUN apk add firefox
RUN apk add py3-pip
RUN pip3 install -U selenium

CMD ["node", "bot.js"]
