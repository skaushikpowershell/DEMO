FROM nginx
COPY ./index.html /usr/share/nginx/html/index.html
WORKDIR /user/share/nginx/html
RUN date +%x_%H:%M:%S:%N >> ./index.html