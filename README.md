Slackish
========
Slackish is small library that lets you convert you simple functions into running slack bots.


Usage
-----
```python
from slackclient import SlackClient
from slackish import Slackish, Command

@Command
def create(campaign, on='Bing')
    Slackish.send("Campaign created succesfully on {}!".format(on))

config = {}
config['BOT_ID'] = None
config['RTM_READ_DELAY'] = 1
config['SLACK_BOT_TOKEN'] = ''
config['SLACK_MENTION_REGEX'] = "^<@(|[WU].+?)>(.*)"
my_bot = Slackish(SlackClient, Command.registry, **config)
my_bot.serve()
```
Instlation Procces
<hr>
<h3>Create your own app</h3> 

Open your slack channel 
Select bots
<img src="info/Selection_001.png">
Create your app
<img src="info/Selection_002.png">

Get the access tokens and connect it to your code
<img src="info/Selection_004.png">

```
config['SLACK_BOT_TOKEN'] = 'Add Your access API Token'
```

after running the code above

check that your app is Active on Slack 
