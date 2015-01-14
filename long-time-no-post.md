# Long time, no post
It's been a while since I've blogged anything.

My industrial placement's kept my quite busy and I haven't really been keeping this blog up to date so I suppose I should give a brief update.

Sunrise is no longer in development, and if it does get carried on at some point then I think it'll be completely overhauled to use NodeJS, MongoDB, and websockets.

Outside of work I haven't really been doing all that much, but I have made a couple of tools for work.

Working with tight memory and storage constraints, I log some of my debugging data in a TLV (Tag, Length, Value) format.

In its simplest representation, this uses a byte to uniquely identify what kind of information is stored, a byte for the length, and the data following. This is brilliant because it uses barely any space, and I can log many more events before I fill my log file and need to stop testing.

The downside is that this is quite unreadable, even with line/column counts etc. To combat this I hacked together a quick tool to show this data as a tree view:

![An image depicting the TLV view's interface with some example data.](http://%current-domain/res/media/tlv-viewer.png)

I also work with converting data between signed/unsigned representations and bytes/shorts/ints, so I made something to convert them too:

![An image of the Primitive Converter program with some example data](http://%current-domain/res/media/prim-converter.png)

(Updating any field with a decimal or hex number changes all other cells)

Well, that's all for now. I'll probably update this if I do anything noteworthy or it's been months since an update again.
