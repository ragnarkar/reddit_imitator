# README
Since Reddit is planning on disabling its API access at the end of June 2023, I'm gonna provide the notebooks I've used to download subreddit data for training the Loras for imitating each sub.  These will be provided "as is" - I've not had the chance to refactor them or to improve the style or fix any bugs or anything.

There are two versions available - a default (DFS) version and a BFS version.  The default version will use DFS to traverse a comment tree to scrape all of the reply comments while the BFS version will use BFS instead.

Generally, you'll want the DFS version for smaller subreddits and BFS for the larger ones.  Also, the BFS version will terminate once it finds 1 million posts or comments so that it won't go on forever.

Note, I don't have a mechanism for resuming a stopped session so you can only hope that you won't lose your connection before it finishes.

One of the top cells will ask for your Reddit credentials which you can store in a key file.  If it doesn't find the key file, it'll ask for them manually.

Note that the notebooks will automatically save the comments it downloads in the Alpaca format in .json for training using the [Alpaca-Lora repostiry](https://github.com/tloen/alpaca-lora).
