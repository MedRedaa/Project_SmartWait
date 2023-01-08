FROM python:3.9
COPY requirements.txt /app/requirements.txt
WORKDIR /app
RUN pip install -r requirements.txt
ADD . /app
CMD ["python", "Run.py", "--prototxt", "models/MobileNetSSD_deploy.prototxt", "--model", "models/MobileNetSSD_deploy.caffemodel", "--input", "videos/example_01.mp4"]