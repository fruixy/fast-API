FROM python:3.11

WORKDIR /usr/src/app
COPY requirements.txt ./
COPY ./src ./src
COPY ./build ./build

RUN pip install --no-cache-dir --upgrade -r ./requirements.txt

EXPOSE 3001

CMD [ "python", "./src/server.py" ]