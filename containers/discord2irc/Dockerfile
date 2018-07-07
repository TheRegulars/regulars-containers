FROM alpine:3.8
RUN apk --no-cache add nodejs npm && \
    addgroup -S discord-irc && \
    adduser -S discord-irc -G discord-irc

RUN npm install -g discord-irc@2.6.1 && mkdir /etc/discord2irc
VOLUME /etc/discord2irc/
WORKDIR /etc/discord2irc/
USER discord-irc:discord-irc
CMD discord-irc --config /etc/discord2irc/config.json
