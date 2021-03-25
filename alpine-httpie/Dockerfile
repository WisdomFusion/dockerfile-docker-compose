FROM alpine

RUN sed -i 's#https\?://dl-cdn.alpinelinux.org#http://mirrors.ustc.edu.cn#g;$ahttp://mirrors.ustc.edu.cn/alpine/edge/main\nhttp://mirrors.ustc.edu.cn/alpine/edge/community\nhttp://mirrors.ustc.edu.cn/alpine/edge/testing' /etc/apk/repositories \
&& apk update \
&& apk add --update --no-cache py-pip \
&& pip3 install --upgrade pip setuptools httpie \
&& rm -r /root/.cache

ENTRYPOINT [ "http" ]

CMD ["--help"]