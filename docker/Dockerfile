FROM python:3
ENV PYTHONUNBUFFERED=1

WORKDIR /app

EXPOSE 8000

COPY src/requirements.txt /app/
RUN pip install -r requirements.txt

COPY docker/entrypoint.sh /app/entrypoint.sh

COPY src/ /app/


ENTRYPOINT ["/app/entrypoint.sh"]
