FROM amd64/ruby:2.6.3
RUN apt-get update -qq && apt-get install -y
ENV DIR=/app
WORKDIR ${DIR}

# install nodejs(LTS)
RUN curl -fsSL https://deb.nodesource.com/setup_lts.x | bash - && apt-get install -y nodejs

# install yarn
RUN npm install --global yarn

# gem
COPY Gemfile ${DIR}
RUN bundle install
