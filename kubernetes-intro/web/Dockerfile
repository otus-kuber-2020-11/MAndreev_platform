FROM python:3.8-alpine
RUN addgroup -g 1001 app \
  && adduser -u 1001 -D -G app app
USER 1001
WORKDIR /app
VOLUME /app
EXPOSE 8000
ENTRYPOINT ["python", "-m", "http.server", "8000"]
