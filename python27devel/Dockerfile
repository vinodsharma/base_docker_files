FROM amazonlinux:2017.03

RUN yum update -y
RUN yum -y install gcc-c++ python27-devel atlas-sse3-devel \
                    lapack-devel python27-virtualenv zip \
                    postgresql-devel mysql-devel docker
RUN /usr/bin/virtualenv venv
RUN source venv/bin/activate
RUN pip install --upgrade --no-cache-dir pip
RUN pip install --upgrade --no-cache-dir sqlalchemy
RUN pip install --upgrade --no-cache-dir psycopg2
RUN pip install --upgrade --no-cache-dir mysql-python
RUN pip install --upgrade --no-cache-dir python-dotenv
RUN pip install --upgrade --no-cache-dir awscli
RUN pip install --upgrade --no-cache-dir boto3
RUN pip install --upgrade --no-cache-dir logdna
RUN pip install --upgrade --no-cache-dir bugsnag
