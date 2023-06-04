FROM docker.io/library/rust:alpine

RUN apk update && apk add git build-base nodejs npm
RUN cargo install create-tauri-app || true