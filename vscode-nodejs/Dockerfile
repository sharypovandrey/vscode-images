FROM nginx:latest
RUN pacman -S nodejs npm
RUN curl -fsSL https://code-server.dev/install.sh | sh
EXPOSE 8000 9000
ENTRYPOINT [ "/usr/bin/code-server", "--bind-addr", "0.0.0.0:9000" ]
