FROM docker.io/library/rust:alpine

RUN apk update && apk add openssh git build-base nodejs npm
RUN cargo install create-tauri-app || true