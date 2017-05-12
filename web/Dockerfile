FROM alpine
RUN apk add --no-cache bash py2-pip \
	&& pip2 install --upgrade pip \
	&& pip2 install flask
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["app.py"]
