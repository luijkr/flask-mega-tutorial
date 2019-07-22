# My first flask application

Creating and deploying a Flask application on AWS.

Resources
- Creating a flask application [Mega Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
- Deploying it to AWS using [Zappa](https://blog.apcelent.com/deploy-flask-aws-lambda.html)

### Prerequisites

Create virtual environment

```
python3 -m venv venv
source venv/bin/activate
```

Install packages and freeze

```
pip install flask
pip install zappa
pip freeze > requirements.txt
```

Setup Zappa

```
zappa init
```

Deploy

```
zappa deploy dev
```

If this doesn't work, try undeploying, and redeploying

```
zappa undeploy
zappa deploy dev
```
