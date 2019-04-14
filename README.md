## Synopsis

Examples for using the Chart.js library in a Flask web application for creating line charts. Also, how to deploy the app with Zappa.

Original code from [Patrick Kennedy](https://gitlab.com/patkennedy79/flask_chartjs_example/tree/master), explained in [his post](https://www.patricksoftwareblog.com/creating-charts-with-chart-js-in-a-flask-application/).

## Install dependencies
Create env:
```
virtualenv ~/chartjs
```

Activate env:
```
source ~/chartjs/bin/activate
```

Install from requirements file:
```
pip install -r requirements.txt
```

## How to run locally
Activate env:
```
source ~/chartjs/bin/activate
```

In the top-level folder, run the development server:
```    
python app.py
```

Go to your favorite web browser and open:
    http://locallhost:5000

## Deploy with Zappa

If it is the first time, configure Zappa:
```
zappa init
```

Once configured:
```
zappa deploy
```

To update deploy with new changes in code:
```
zappa update
```

To delete the services in AWS after testing:
```
zappa undeploy
```
