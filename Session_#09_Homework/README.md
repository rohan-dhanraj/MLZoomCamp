# Cats Dogs Image Classification using CNN
Files:  
1. [Notebook](./notebook.ipynb)
2. [Lambda Function](./lambda_function.py): Serverless
3. [Model](./Dockerfile)
4. [Dependency](./requirements.txt)
5. [Test file](./test.py)

## How to run the Lambda Function(Serverless) containing the Model?
```bash
docker build -t cats-dogs .
docker run -it --rm -p 8080:8080 cats-dogs:latest
```

## How to test the Model?
After running the [Dockerfile](./Dockerfile)
Run the [Test Script](./test.py)
```bash
python test.py
```
