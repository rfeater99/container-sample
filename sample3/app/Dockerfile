FROM ruby:2.5.1

RUN mkdir /app
WORKDIR /app

RUN apt-get update && apt install -y nodejs
RUN curl -sL https://ibm.biz/idt-installer | bash
RUN gem install rails -v 5.1.6

RUN git clone https://github.com/rfeater99/hello_app.git ./

RUN bundle install --without production

