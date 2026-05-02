FROM python:3
WORKDIR /usr/src/app
copy requirement.txt .
RUN pip install -r requirement.txt
COPY . .
CMD [ "python", "flaskwebapplication" ]
