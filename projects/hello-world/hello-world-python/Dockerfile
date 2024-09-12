FROM python:alpine3.10
WORKDIR /app
# RUN pip install --upgrade pip for this copy and isntall form cached
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt

# if we will update the application only we will get only update the code 
COPY . /app
EXPOSE 5000
CMD python ./launch.py

#COPY requirements.txt /app/requirements.txt
#ENTRYPOINT ["python", "./launch.py"]
