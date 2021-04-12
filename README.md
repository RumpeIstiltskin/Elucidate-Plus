## What is Elucidate Plus?
Elucidate Plus is an in-game chat translator and communication software. It allows players to seamlessly translate in-game chat messages and type back in the language detected. The software itself is external but is mainly controlled through the Steam Overlay’s browser.

## Why is it using the Steam Overlay?
The Steam Overlay is internal, safe with anti-cheat systems, and can be injected into any game added to the Steam library. It also has a built-in screenshot function, which is programmatically used, and works on all games regardless of how they are rendered. Controlling Elucidate Plus through the overlay is a click away. 
How the game is rendered is incredibly important because Elucidate Plus needs a screenshot to execute the Optical Character Recognition process. 
For an example, some games use the video-adapter’s hardware overlay. This is a buffer that software can write to which provides hardware acceleration. By nature, it is just a simple rectangle that the video-adapter fills in with the output image in hardware. 

As a result, Windows API or external screen capturing methods do not have access to the rendered image, and so the handler cannot capture it. The Steam Overlay having an internal nature bypasses this.
Data Extraction

Elucidate Plus uses OCR as its main method to extract the data from the game. It doesn’t waste processing power by extracting messages that are already in a language you can read, as an example, if I were using Elucidate Plus in English, it detects and only extract messages that aren’t in English. 


## Using Elucidate Plus | Steam Overlay
#### ROBLOX
This capture shows the extraction and translation for one player typing in German.
