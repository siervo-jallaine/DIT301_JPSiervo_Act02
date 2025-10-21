**REFLECTION**

**1. What did you observe about the app lifecycle when switching between screens or minimizing the app?**

   Honestly, watching the Logcat messages was a bit confusing at first with all the text scrolling by.
But after navigating back and forth a few times, I started to see a pattern. It was interesting to 
see that when I went to the second screen, the first one didn't just vanish; it paused and then stopped 
in the background. Then, when I hit the back button, the app didn't have to remake the first screen from
scratch, it just restarted it.

**2.What did you learn about activity management in Android?**

   The concept of the "back stack" was the big thing that finally clicked for me. Before this, I didn't really
get why one screen would be destroyed while the other one just waited. Thinking of it like a deck of cards really
helped. Every time a new screen opens, a new card is placed on top of the deck. When you hit the back button, you're
just taking the top card off and throwing it away. It's a simple but really smart way to make sure you don't lose 
your place when you're moving between screens.
