FROM python 
  
RUN useradd -ms /bin/bash pyusr

RUN mkdir -p /home/pyusr/app/ && chown -R pyusr:pyusr /home/pyusr/app

WORKDIR /home/pyusr/app

COPY * ./

USER pyusr

RUN pip install twilio

COPY --chown=pyusr:pyusr . .
