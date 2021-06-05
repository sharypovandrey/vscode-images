FROM tiangolo/uwsgi-nginx-flask:python3.8
RUN apt update && apt install -y ca-certificates
RUN curl -fsSL https://code-server.dev/install.sh | sh
EXPOSE 8000 9000
ENTRYPOINT [ "/usr/bin/code-server", "--bind-addr", "0.0.0.0:9000" ]