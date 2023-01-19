FROM python:3
LABEL Maintainer="Gabe Holmes"

COPY ./src/ /app/

RUN apt-get update && apt-get install -y \
    python3-pip

RUN pip install --pre scapy[basic]
CMD ["chmod +x /app/scapy"]

ENTRYPOINT ["/app/scapy"]
