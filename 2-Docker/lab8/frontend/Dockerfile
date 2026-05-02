FROM python:3.11.15-slim-trixie
WORKDIR /app
COPY . . 
RUN pip install -r /app/requirements.txt
EXPOSE 5000
CMD [ "python", "app.py" ]