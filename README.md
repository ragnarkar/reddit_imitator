# reddit_imitator

## Intro

This repository lets you simulate having a Reddit post or comment replied by people from a particular subreddit.  I've trained models for various subreddits using the best rated comments in the sub.

## How to install

First, open the **[Reddit_imitator.ipynb](https://github.com/ragnarkar/reddit_imitator/blob/main/Reddit_imitator.ipynb)** file and click the "Open in Colab" link at the top.

Second, click the arrow below the "Initial Setup" cell. Then go to the 2nd cell and pick a subreddit. Run that cell when the first cell is done running.  (You do not need to restart the runtime if you're prompted to do so.)

Then once the 2nd cell is done running, go to the bottom cell and run that.  You'll eventually get two links; click on the 2nd link that is longer and appears more like gibberish.  That'll open the interface.

## How to run

Once you have the interface open, the default prompt has been loaded where it tries to generate a new post that's in the spirit of that sub. Click on the gold "Generate" button and it'll start generating a new post. There are 4 options when you open the "Prompt" menu near the bottom left of the screen:

- **CreatePost** and QA all do the same: you can have it generate a random post. **Do not edit anything in the prompt window, at least when you're first starting out**.  Later on, once you get the hang of it, you can try providing a title and have it fill in the self text by adding a [Title:] (your title goes here) bit and also a [Selftext:] bit.
- **ReplyComment**: Select this and then select the "(Comment text goes here)" bit and paste your comment there to replace it before running Generate.
- **ReplyTopPost**: If you want a reply to a top post which has a title and maybe some self text, select this option and paste the title right after the [Title:] bit.  **If there's no self-text, leave the [Selftext:] bit in but delete any text between that and the ### Response part**.

Also, if you're not satisfied with the response, you can always have it generate another one by hitting the Generate button again. If it's in the middle of generating, be sure to hit Stop first. If you like what it generated but it stopped abruptly, hit the "Continue" button.

## How to exit

If you want to switch to a different subreddit, click the stop icon to the left of the 3rd cell, then go back to the 2nd cell and pick another sub before rerunning it.  Then run the 3rd cell and click the 2nd link to open a new interface.

If you're done playing with this for the day, you'll want to properly exit it so that the resources are returned to Google. Go to the Runtime menu above and select the "Disconnect and Delete Runtime" option.  If you don't do this, the program will run for several hours until it gets shut down by Google, and if you do this often enough, Google will severely limit the amount of time you can use this everyday.

## Where to learn more

If you like this demo and want to learn more about Generative AI, particularly Large Language Models or to get further support, you can head over to the [text-generation-webui page](https://github.com/oobabooga/text-generation-webui). This program is the main engine that drives my reddit imitator.

## Disclaimer and rules

This code and models are provided as is. I'm not responsible for any physical or mental harm caused to you or others for using this as well as any other 2nd, 3rd or higher order consequences as a result of your use of this program. The instructions here may not always be up to date either.

I urge you to use these models responsibly.  Having a laugh yourself or showing them off to your friends is great.  Abusing them isn't.  Abuse includes:

- Commercial use: some of the models and data used to build this program are not licensed for commercial use so you cannot use these for any direct financial gain.
- Hate speech and harassment: please don't use these models to generate hate speech or to harass other people (or bots).
- Spam and excessive posts: I don't explicitly forbid you from building a bot using these models but please don't use them to spam or generate an excessive amount of posts on Reddit or anywhere else on the Internet.
