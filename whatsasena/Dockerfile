FROM fusuf/whatsasena:latest

RUN git clone https://github.com/phaticusthiccy/WhatsAsenaDuplicated /root/WhatsAsenaDuplicated
WORKDIR /root/WhatsAsenaDuplicated/
ENV TZ=Europe/Istanbul
RUN npm install supervisor -g
RUN yarn install --no-audit
RUN apk add python3

CMD ["node", "bot.js"]
