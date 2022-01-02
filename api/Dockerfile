#バックエンド実装
FROM ruby:2.7.0

# -qq : ログ表示を減らす
# -y : 常にyesを返す
RUN apt-get update -qq && apt-get install -y mysql-server libmysqlclient-dev
RUN mkdir /myapp
WORKDIR /myapp
ADD Gemfile /myapp/Gemfile
ADD Gemfile.lock /myapp/Gemfile.lock
RUN bundle install
ADD . /myapp
