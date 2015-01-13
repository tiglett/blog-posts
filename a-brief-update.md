# A brief update
I've been quite busy since my last post, and have written a Maven plugin and a library in Java.
I'll go over these in their own dedicated posts soon, but here's a quick description of them both:

## Maven Plugin

To help with cross-platform compatibility and to increase the robustness of our Javacard build system, I wrote a Maven Mojo plugin.
This allows Javacard applets to be built with Sun's converter programmatically, and properly resolves dependencies.

## CAT-TP Library
Another project I've been working on is an implementation of the [CAT-TP Bearer Independant Protocol](http://www.etsi.org/deliver/etsi_ts/102100_102199/102127/06.06.00_60/ts_102127v060600p.pdf). This involves classes which provide synchronous and asynchronous bindings to allow data to be sent over a networking using CAT-TP simply.

## Blog
Another thing I've decided to do is switch from Wordpress to my own blogging solution.
Wordpress is huge and contains a lot of functionality I'll never use, so I've made a (mostly) client-side blog implementation.
The blog itself (and its posts) are stored on git. Posts are written in markdown and the client transforms these into HTML with the use of [markdown-js](https://github.com/evilstreak/markdown-js). Updating my blog now just involves doing a `git pull` after adding or updating posts on the post repository.
