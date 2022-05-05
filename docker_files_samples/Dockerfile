FROM python:3.8-alpine

RUN groupadd -g 1000 flask_users 
RUN useradd -u 1000 -ms /bin/bash -g flask_users flask_users

COPY --chown=flask_users:flask_users ./requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip install --no-cache-dir -r requirements.txt

COPY --chown=flask_users:flask_users . /app

USER flask_users

ENTRYPOINT [ "python" ]

CMD [" < .py exec file name> "]

EXPOSE 8080




