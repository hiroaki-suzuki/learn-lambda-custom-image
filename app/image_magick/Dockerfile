FROM public.ecr.aws/lambda/python:3.12-x86_64

RUN dnf install -y ImageMagick

COPY app.py requirements.txt ./

RUN python -m pip install -r requirements.txt -t .

CMD ["app.handler"]
