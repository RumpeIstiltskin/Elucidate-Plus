# Elucidate Plus | Proof of Concept | Last Updated: 19th April
This update acts as a project announcement and briefly covers the core of Elucidate Plus. Details and explanations for each implementation will be in the next update, as a lot is still being finalised. 

## What is Elucidate Plus?
Elucidate Plus is an in-game chat translator and communication software. It allows players to seamlessly translate in-game chat messages and type back in the language detected. The software itself is external but is mainly controlled through the Steam Overlay’s browser.

## Why is it using the Steam Overlay?
The Steam Overlay is internal, safe with anti-cheat systems, and can be injected into any game added to the Steam library. It also has a built-in screenshot function, which is programmatically used, and works on all games regardless of how they are rendered. Controlling Elucidate Plus through the overlay is a click away. 

How the game is rendered is incredibly important because Elucidate Plus needs a screenshot to execute the Optical Character Recognition process. 

For an example, some games use the video-adapter’s hardware overlay. This is a buffer that software can write to which provides hardware acceleration. By nature, it is just a simple rectangle that the video-adapter fills in with the output image in hardware. 

As a result, Windows API or external screen capturing methods do not have access to the rendered image, so the handler cannot capture it. The Steam Overlay having an internal nature bypasses this.

## Steam Overlay - Browser Implementation | Part I of II
<a href="https://www.youtube.com/watch?v=RiF1632eTu4">Watch Video (Part I)</a>

## Stean Overlay - Chat Bot Implementation | Part II of II
<a href="https://www.youtube.com/watch?v=5DJR1EOKm0w">Watch Video (Part II)</a>
