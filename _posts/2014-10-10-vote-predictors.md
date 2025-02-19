---
title: Vote Predictors
author: Ali
layout: post
categories:
  - Research
---
Jure Leskovec has been teaching CS 224W this quarter, and a number of his lectures have used research questions to illustrate the concepts and models that he's been teaching. It's been an interesting way of surveying the kind of research he does, which is hopefully informative for anyone planning on rotating into Jure's lab (e.g. me). Recently, he talked about a question of predicting Wikipedia admin elections, and described the results of some research wherein he found that, by accounting for voter-candidate similarity and for status difference (again, between the voter and the candidate), you can predict the outcome of the election just by knowing *which* 5 people came out to vote first with ~70% reliability; this, without knowing **for whom** they voted. Knowing their votes, you can predict with approximately 85% accuracy. By looking at voters 1-10 (again, not the votes, just the turnout), accuracy rises to 75%, after which point accuracy rises negligibly - even with all voters.

This was really fascinating, but ~70% is not *great*, and there's certainly room for improvement. I asked if looking at different subsets of votes (voters 2-6 instead of 1-5, for instance) would yield different predictive accuracy. It didn't seem like this had been pursued, but I suspect that sock puppet voters and the like might be less representative of the overall outcome for an election, making voters 1-n (where n is small) more noise than signal.

If anyone is interested in following up on this question, I'm certainly interested in seeing if I'm right.