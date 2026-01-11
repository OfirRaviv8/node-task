FROM alpine:3.19
RUN apk add --no-cache unzip bash
WORKDIR /app
COPY myzip/myapp.zip /tmp/app.zip
RUN unzip /tmp/app.zip -d /app && rm /tmp/app.zip
RUN chmod +x /app/main.sh
CMD ["bash", "-c", "/app/main.sh"]
