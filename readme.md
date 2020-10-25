# Mapreduce programming with Python

This is a Python projects that contains two MapReduce applications:
    - Word Count
    - Flights By Carriers

## Assumption

Need to use cisc-525-util repository to:
    - start up hadoop
    - prepare data (make sure you have the data downloaded and stored in the right place)
    - verify data loaded correctly

## Run Word Count MR application

```shell script
./word_count_run.sh /user/student/shakespeare/tragedy/othello.txt /tmp/othello
```

### Run  MR application for flights by Carrier
./fbc_run.sh /user/student/airline/2000.csv /tmp/2000
###

### Run MR application for flights by Origin
./fbO.sh /user/student/airline/2000.csv /tmp/py-airline-carriers-2000
###

### Run MR application for flights by Destination
./fbD.sh /user/student/airline/2000.csv /tmp/py-airline-Destination-2000
###


## Unit test

```shell script
pip3 install pytest
```

```shell script
pytest 
coverage run --source=app -m pytest 
coverage report -m
```

- include these in the __init__.py:
````python
import sys
sys.path.append('.')
````
