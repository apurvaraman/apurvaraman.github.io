---
layout: post
title: Mass Feeds
---

# Mass Feeds | Miranda Lao and Apurva Raman

## About the project
Inspired by [@trumps_feed](https://twitter.com/trumps_feed?lang=en), we have compiled the “Twitter feeds” of various candidates for public office in the Fall 2018 election. Many people use their social media feeds as a main source of news and public opinion, and we thought it would be valuable to see what our candidates choice in “following” would say about their platforms and beliefs.

On Twitter, you generally have ability to see what people post, but not necessarily the influences behind those thoughts. Since lists are presented entirely chronologically, there is room to question and explore what people might be seeing and how that influences what they post. This is especially applicable and pertinent to our public officials.

## Our process
Originally, we thought of creating an aggregate account for Oliners on Facebook. We would give multiple Oliners access to this account and see the amalgamation of what they had posted. In some ways, this would give us a way to to see how the Facebook algorithm stereotyped a collective “Oliner”. We were also interested in seeing the interpersonal connections and how people’s offline connections were influenced by a different online connection (from what they would normally experience).

### Manual interactions vs bots
We started by manually adding the accounts Sen. Elizabeth Warren follows to a list. Twitter lists show you the tweets of members of that list in chronological order, so this is somewhat of an approximation of her Twitter timeline. It’s worth noting that after adding the first 30 or so accounts to a list in rapid succession, Twitter required a two-factor authentication to ensure that we were not bots. After confirming that we were not in fact a robot, we then could add more accounts to a list.

We wrote [a script](https://github.com/apurvaraman/mass-feeds) to add people to lists automatically, because both Geoff Diehl and Shiva Ayyadurai (the other two senatorial candidates on the ballot) follow over 2000 accounts. We ran into a few issues when we did this. One was that we needed approval from Twitter to use their api, which took a few days. Despite this approval process, Twitter doesn’t just rate limit api calls but also stops you from performing certain actions (like adding people to lists) if you do them a certain amount within a given time window. We also found many of the accounts followed by Geoff Diehl blocked us automatically when we added them to the list. We don’t know how many accounts this is, because we’ve also hit the limit for how many accounts we’ve been adding in a 24 hour period a few times.

## Insights
We have had some strange interactions with our account—auto-blocking being one of them—where we’re not sure if the people we’re interacting with are bots, humans, or humans using automation tools with Twitter. This gets at a larger question about how real any of this is:
- Are these politicians’ accounts handled by a press team or social media manager?
- Do they look at their Twitter feed?
- Do they have bots running?
- Are the people they follow real?
- How real is comparing a Twitter list to a Twitter feed?

This last question is an interesting one. Twitter lists take everyone you follow on that list and show you *all* their tweets, in chronological order. If you just follow them, you see some of their tweets, not necessarily in chronological order, based on what Twitter’s algorithm decides you should see. In this sense, because we don’t interact with tweets in the same ways as each of the politicians do, we might not get shown the same tweets. With the list, we see a superset of the tweets that a politician may see on their feed, but we see them in different amounts and proportions. Neither representation is perfectly accurate to the actual feed.
