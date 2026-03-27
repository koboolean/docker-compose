FROM redmine:latest

# plugins 포함
COPY plugins /usr/src/redmine/plugins

# themes 포함
COPY themes /usr/src/redmine/themes

# 작업 디렉토리
WORKDIR /usr/src/redmine

# 포트
EXPOSE 3000

# 실행 (핵심)
CMD ["rails", "server", "-b", "0.0.0.0"]
