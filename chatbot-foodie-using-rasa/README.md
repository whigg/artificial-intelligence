# Simple Chatbot using Rasa.ai

###### Documentation in progress ...

Using RASA NLU version `0.12.3`

Using RASA Core version `0.10.1`

Using Python version 3.6.8

## How to Run:


## What to Install

#### Install Rasa NLU

`$pip install rasa_nlu`

#### Install Rasa Core

I am installing from Git.

```

$git clone https://github.com/RasaHQ/rasa_core.git
$cd rasa_core
$pip install -r requirements.txt
$pip install -e .
```


#### How to find rasa_core and rasa_nlu version

```
$python -c "import rasa_nlu; print(rasa_nlu.__version__);"
$python -c "import rasa_core; print(rasa_core.__version__);"
```


## How to do HTTP/REST

`$python -m rasa_core.server -d models/dialogue -u models/nlu/default/customernlu/ --debug -o out.log --cors *`

On a separate terminal, run CURL

`$curl -XGET localhost:5000/'`

It should output

`HTML File`


## Further Improvements: