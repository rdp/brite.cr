![Lightbulb!](logo.png)

# Brite Site Duex


## A Little History

Back in the days when I was in the churning deeps of Ruby development, I created an early
static site/blog engine called Brite. It was unique in a number of ways. For starters
post files actually had a `.post` extension. Imagine that. It also supported multi-format
documents via my Neapolitian gem. Markdown and Textile in one page. Holy cow! Well Jekyll
came along and the world mostly moved to Markdown. Around that time I had started writing
my blog posts in a github wiki and, after wrestling with some foolish overwrought approaches,
was able to write a small plugin for Jekyll to render my wiki pages just fine. Things were
pretty good.

Fast forward to 2016 and Jekyll has failed me for the last time! My plugin is now broke 
because of changes to Jekyll, and Bundler is keeping me locked in gem dependency hell. So
I decided to try some alternatives. I ended up taking a spin on Hugo written in Go, Obelisk
written in Elixir, and Cryogen which is written in Clojure. Hugo seemed promising, but it 
soon started giving me fits. Themes are in bad shape and it is difficult to extend. Obelisk
showed promise, but it had no themes at all. You get blank page. So it just wasn't far enough
along. Of the three, Cryogen worked the best. With only a little conjoling I was able to get
my site up, it looked pretty good and was fully functional. I was about a stones throw from
commiting to it -- after all I've always had a soft spot for Lisp. But there was this nagging
voice in the back of my mind that I could not shake. "They are doing it wrong."


## A New Approach

Brite takes a fairly different approach from all the other copycat static site generators
out there. First of all it uses a pipeline. Some other tools use a pipeline. It's a smart
approach, but unlike the others, Brite's pipeline is composed of indiviual tools. Any one
of which can be replaced if need be, without restriction on language or dependencies.
Don't like Brite's built-in Markdown renderer? Just replace that part with a shell script
that uses Pandoc. Fine by us. It is your site after all. The `brite` command line tool
is really little more than a lightweight wrapper that manages this pipeline.

More to come...

### Features

* Unix philopsophy
* Statically compiled 
* Extensible pipeline
* Mustache Templates
* Markdown Format
* HCard support
* RSS/Atom feeds
* Easy Themes

**Maybe Features**

* Dynamic Javascript site (in addition to full static)
* Constraint-based Stylesheets


## Getting Started

Right now it's all development hoss. So keep you pants on and will get wrangling pony as soon
as we can.


## Copyrights

Brite Site Duex (c) 2016 OpenBohemians

