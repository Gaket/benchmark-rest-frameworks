FROM python:3.13-slim
RUN apt-get update && apt-get upgrade -y
WORKDIR /app
COPY . .
RUN python -m venv /venv
ENV PATH="/venv/bin:$PATH"
RUN pip install -U pip
RUN pip install -r requirements.txt
ENTRYPOINT [ "python" ]
CMD ["app.py"]