# inferno-slate-compat
https://github.com/RB-bro/inferno-slate-compat

Attempting to get slate and inferno to work together


I'm trying to start with the simple demo from the Slate.js page using Inferno instead of React for rendering. My barebones 
repo works fine with React, but does not render with inferno-compat.  I've turned on localStore.debug = 'slate:*' 
and discovered that the logs match up between React and inferno up until the the leaf render debug message. It 
appears in the React version, but not the Inferno one.

Everything behaves the way it does when using react to render, including updating the dom, 
as you can see similar html generated in the page (minus the editor),
but it seems as if the leaf constructor is never invoked.

I've stepped through a lot of the Slate code in the Chrome DevTools, 
but have not been able to isolate the problem. 
How should I proceed to find the problem so I can make a patch?
