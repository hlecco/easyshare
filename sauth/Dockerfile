FROM python:3.6-slim-buster
COPY sauth /opt/sauth

RUN pip install click

WORKDIR /opt/sauth

ENV USERNAME admin
ENV PASSWORD admin

CMD ["sh", "-c", "python sauth.py --dir /var/share $USERNAME $PASSWORD 0.0.0.0 8080"]
