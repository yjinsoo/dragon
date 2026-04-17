FROM nginx:stable-alpine

# 1. Nginx 설정 파일 복사 (Reverse Proxy 설정 포함)
# 로컬의 default.conf 파일을 Nginx 설정 디렉토리로 복사
COPY conf/default.conf /etc/nginx/conf.d/default.conf

# 2. HTML 파일 복사
COPY html/index.html /usr/share/nginx/html/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
