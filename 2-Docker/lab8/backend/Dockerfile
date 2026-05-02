FROM python:3.11.15-slim-trixie
WORKDIR /app
COPY . .
RUN pip install flask 
EXPOSE 5000
CMD [ "python", "app.py" ]