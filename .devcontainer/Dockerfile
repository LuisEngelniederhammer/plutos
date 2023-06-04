FROM docker.io/library/rust:buster

#RUN apk update && apk add openssh git build-base nodejs npm pkgconfig libressl-dev libsoup-dev webkit2gtk-dev
RUN apt update &&\
    apt install -y libwebkit2gtk-4.0-dev \
    build-essential \
    curl \
    wget \
    libssl-dev \
    libgtk-3-dev \
    libayatana-appindicator3-dev \
    librsvg2-dev \
    git \
    ssh \
    npm
RUN cargo install tauri-cli

RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
RUN export NVM_DIR="$HOME/.nvm" && [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" && nvm install node --lts