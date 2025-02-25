FROM python:latest

RUN groupadd vscode \
    && useradd -m -g vscode -s /bin/bash vscode

RUN apt-get update && \
    apt-get install -y build-essential wget openssl cmake && \
    apt-get install -y gcc g++ curl libmcrypt-dev default-mysql-client

RUN apt-get install -y libssl-dev libffi-dev libmariadb-dev-compat libmariadb-dev libtcmalloc-minimal4 libgoogle-perftools-dev

RUN apt-get install -y dnsutils telnet net-tools iproute2

CMD ["/bin/bash"]
