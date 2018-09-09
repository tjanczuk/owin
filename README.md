Looing for owin? The project has been renamed Edge.js and moved to https://github.com/tjanczuk/edge 
====

Why was that done? The owin project started off as a way to host .NET [OWIN](http://owin.net) applications as express.js request handlers and connect middleware. It has since become more generic to include broader scenarios of running node.js and .NET code in-process. The old name no longer captured the new scope, and caused some confusion with the actual OWIN specification. 

## So what is Edge.js anyway?

An edge connects two nodes.

The Edge.js connects node.js and .NET. 

It is a way to run node.js and .NET in one process. 

## What happens if I cloned owin?

You can keep your files, but you need to update your remote URL:

```
git remote set-url origin git@github.com:tjanczuk/edge.git
```

## What happens if I forked owin?

You will likely need to update your `upstream` remote url to point to edge URL like above. You may also consider changing the name of your fork, but that is not required. 

Any work you have been doing in your fork is unaffected, and you can still do pull requests to the edge repository via GitHub.

## What happens with npm?

You will now install the edge.js module with

```
npm install edge
```

All existing releases of owin will remain in npm, but new releases will ship under the `edge` module name.

## Questions? Feedback

[@tjanczuk](http://twitter.com/tjanczuk)
