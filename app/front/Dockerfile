FROM nginx:alpine

COPY . /usr/share/nginx/html
COPY ./entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENV WS_BACK_URL=http://localhost:8080

EXPOSE 80

ENTRYPOINT ["/entrypoint.sh"]

CMD ["nginx", "-g", "daemon off;"]
