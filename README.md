# Grimoire

A new experiment in creating a custom search engine.

## General Theory

### Inputs

Grimoire is based around inputs - right now I'm thinking about a few different
inputs:

1. Raindrop - pulling indexed sites from bookmarks
2. Inoreader - pulling indexed sites from a feed reader
3. Browser extension - pulling indexed sites from previously visited sites
4. Algorithms / Generators - custom algorithms, a la Bluesky, for finding
   things.

### Transforms

Transforms take inputs and parse them into specific formats. I've got a few
ideas about what this might mean.

#### LLM / LangChain

It would be really nice to be able to say "find me a website that I visited in
the last few weeks with information about X topic" and have the search engine
return some results.

I'm not extremely interested in LLM summarization or consolidation - I want the
actual source material, not auto-completed summaries.

#### Tokenized strings

More straightforward search engine abilities - search for a thing, get some
things back.

### Outputs

First output is going to be just a basic search engine, a list of pages and what
is on them.

Eventually some parsing of structured data / production of rich results would be
nice. Giving the tool access to different services could also return results
from those services - email, bookmarks, browser history, etc could all be
rendered differently.


## Tech Stack

Nothing has be built yet, but I'm considering:

### NextJS for Frontend

### Elasticsearch / Similar for full text indexing

## Goals

### Tiny

Should be easy to deploy / run on any machine.

### Scalable

Should be scalable to whatever your needs are. More inputs shouldn't impact the
performance exponentially.

### Smart

### Useful

### Connected

No matter where this is deployed or how, it should be connected to every other
node. Similar ideas: ActivityHub, Federation, etc
