FROM alpine

# use mirrors.ustc.edu.cn as repo mirror instead

RUN sed -i 's#https\?://dl-cdn.alpinelinux.org#http://mirrors.ustc.edu.cn#g;$ahttp://mirrors.ustc.edu.cn/alpine/edge/main\nhttp://mirrors.ustc.edu.cn/alpine/edge/community\nhttp://mirrors.ustc.edu.cn/alpine/edge/testing' /etc/apk/repositories \
&& apk update \
&& apk add --no-cache mysql-client \
&& rm -r /root/.cache

ENTRYPOINT ["mysql"]
