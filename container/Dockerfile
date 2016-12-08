FROM ubuntu:16.04
RUN apt-get update
RUN apt-get install -y python-pip
RUN pip install django==1.9
RUN django-admin.py startproject demo .
ADD views.py /demo/
ADD urls.py /demo/
CMD ["python","manage.py", "runserver", "0.0.0.0:8000"]

