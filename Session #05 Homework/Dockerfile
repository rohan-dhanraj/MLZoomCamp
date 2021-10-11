FROM agrigorev/zoomcamp-model:3.8.12-slim

RUN pip install pipenv

WORKDIR /app

COPY ["Pipfile", "Pipfile.lock", "./"]

RUN pipenv install --system --deploy

COPY ["app.py", "model1.bin", "dv.bin", "./"]

EXPOSE 8080

ENTRYPOINT ["gunicorn", "--bind=0.0.0.0:8080", "app:app"]