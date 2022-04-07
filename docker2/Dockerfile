FROM python:3.8
COPY . .
RUN pip install -r /stocks_products/requirements.txt
RUN python3 /stocks_products/manage.py migrate
CMD ["python3", "/stocks_products/manage.py", "runserver", "0.0.0.0:8000"]
