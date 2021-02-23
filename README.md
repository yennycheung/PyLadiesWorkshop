# Getting Started with Rasa
Hey all, welcome to the Getting Started with Rasa Workshop with PyLadies Hamburg. Below is a step-by-step guide on the workshop activities. Have fun! If you wish to follow along, this is the [link](https://docs.google.com/presentation/d/12BK1abl5EOR0aRN9kUVJ27AFPDpTcNBSl9YHKmmeI78/edit?usp=sharing) to the slides.

## Task 0: Add NLU data to the Subscription Bot
* Go to Rasa playground [here](https://rasa.com/docs/rasa/playground/), it is an interactive shell you can play with on the browser. On the page, you could see there is a pre-built subscription bot. Press `Train` and talk with the bot! We will refine it by adding more NLU data to the subscription bot on the page.

## Task 1: Add an intent to the Subscription Bot
* On Rasa playground [here](https://rasa.com/docs/rasa/playground/), we will add an intent called `bot_challenge`. We will do that by adding the intent and some examples in `NLU data`, then we will add a response `utter_bot_challenge` under the `Responses` tab. And then add this step to the `Stories` tab. Now it's your turn to add another intent! 

## Task 2: Download the Subscription Bot project from Rasa playground
* On the same page [here](https://rasa.com/docs/rasa/playground/), press `train` if you haven't yet, then you'll see that the greyed out `Download project` button becomes purple, save the project to your machine.
* Navigate to the directory with your subscription bot project, then follow the [step-by-step installation guide](https://rasa.com/docs/rasa/installation#step-by-step-installation-guide). The guide uses `venv` to set up your virtual environment, if you're more used to `conda` you can follow the instructions below to replace `step 2`.
```
conda create -n rasaenv
# the environment should be activated now
# if not, type: source activate rasaenv
```
If you're getting errors, updating conda might help, run: `conda update -n base -c defaults conda`
