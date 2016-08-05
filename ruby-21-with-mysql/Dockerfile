FROM ruby:2.1.2-onbuild
# nodejs is used to provide a js runtime for Rails apps etc
RUN apt-get update && apt-get install -y mysql-server nodejs
RUN service mysql start
RUN gem update --system
RUN gem install bundler
RUN bundle config build.nokogiri --use-system-libraries
