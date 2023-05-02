## Mission

The mission of CheckBuddy is to help public discouse being based on honesty and facts.

## How does it try to accomplish it ?

It does this by helping the consumers of information to assess if claims in a piece of content are solid (sourced, referenced, and that those references are indeed consistent with those claims) 

Beyond the immediate help provider to the user, the tool can offer, (by its recurring / graph-like essence) new data mining opportunitied to understand how information flows, and where it is corrupted.

We believe that this tool can make information producers more accountable, and help consumers discriminate between good and bad information.

This approach is complementary to usual "fact-checking", it does not pretend to etablish a universal truth or a list of verified facts, but to assess the rigour and honesty of the autor.

The drawbacks of usual fact-checking are:
* Requires manual labor for each information
* Always late
* Out of context (the user must look for the fact-checking)
* Depends on the trust of the user
* Depends on the quality and objectivity of the human fact-checker

By contrast, this tool is:
* Automatic
* Real time
* In context
* Gives feedback direclty verifiable by the user
* Depends on the quality of the model and of the annotated dataset, which can be assesed and refined incrementally

## How it works

CheckBuddy is both an app (for mobile) and a navigator plugin (for desktop) where the user can:
* list claims in the article
* verify if those are sourced / referenced
* verify if the provided references are consistant with those claims
* verify the quality of those references (by the same metrics)
* Navigates directly where the claim is substantiated inside those references
* get a fast aggregated score to evaluate the quality of a piece of conent, (including elements like percentage of confirmed claims, average quality of sources...)

## Proof Of Concept

An API with:
* As input: the url of an article
* As output: a JSON with a list of triplets (claim, source, reference)


## Labelling

We must first define what consistute a claim to annotate consistently

## Dataset

https://paperswithcode.com/dataset/fever


## Model

type bert avec classification des token, ou token est:
* source
* reference
* claim

comment les associer ensemble ?
https://paperswithcode.com/sota/relation-extraction-on-docred
https://github.com/youmima/dreeam
