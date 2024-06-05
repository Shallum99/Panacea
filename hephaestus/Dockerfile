# 
FROM python:3.8

# 
WORKDIR /hephaestus

# 
COPY ./requirements.txt /hephaestus/requirements.txt

# 
RUN pip install --no-cache-dir --upgrade -r /hephaestus/requirements.txt


COPY ./sql_app /hephaestus/sql_app
# 
CMD ["fastapi", "run", "sql_app/main.py", "--port", "80"]


# sudo docker build -t panacea .
# sudo docker run --network host -d --name mypanacea panacea
