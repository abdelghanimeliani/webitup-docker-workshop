FROM python:3.10.9
WORKDIR /api
COPY ./ /api
COPY ./saved_models /api

RUN pip install --upgrade pip
RUN pip install -r requirements.txt
RUN pip install protobuf==3.20.*
RUN pip list
CMD [ "python" ,  "main.py" ]
EXPOSE 8000