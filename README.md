# taskgv
Generates a pretty, directed graph of [Taskwarrior](http://taskwarrior.org) projects, tags, and tasks. _Has, thus far, only been tested on OS X._

Things end up looking kinda like this:

![](exgraph.png)

Arrows show implication, so they point from projects to tasks, and from tasks to projects. That is, projects _include_ tasks and tasks _include_ tags.

Projects are represented by large circles, tasks by colored rectangles, and tags by uncolored squares.

## Requirements

* Python

* Taskwarrior

* [Graphviz](http://www.graphviz.org/)

## Usage

When placed in your $PATH, `taskgv.py <filter>` opens a graph of your business, filtered by Taskwarrior `<filter>`.

### Credit

This script is derived from [graphdeps.py](http://taskwarrior.org/projects/taskwarrior/wiki/ExternalScripts#graphdepspy).
