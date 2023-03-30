FROM python:3.10.9
WORKDIR /api
COPY ./ /api

RUN ls

RUN pip install --upgrade pip
RUN pip install -r requirements.txt
RUN pip install protobuf==3.20.*
RUN pip list
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
EXPOSE 9876