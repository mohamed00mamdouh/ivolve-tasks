FROM python:3.11.15-slim-trixie
WORKDIR /app
RUN pip install flask
COPY . . 
EXPOSE 8080
CMD [ "python", "app.py" ]