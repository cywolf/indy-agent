FROM bcgovimages/von-image:py36-1.8-0

COPY requirements.txt .

RUN pip install --trusted-host pypi.python.org -r requirements.txt

COPY . .

ARG PORT

ENV PORT=${PORT}

EXPOSE $PORT

CMD python3.6 indy-agent.py $PORT
