
My project began with a simple question: 
*Could I, with very little technical background, create a script (the simplest type of software program/app) that would let me get the text of a podcast I just listened to?*

### Background
The whole idea started when I was listening to a [podcast about GLP-1 drugs](https://www.theringer.com/podcasts/plain-english-with-derek-thompson/2025/09/16/if-glp-1-drugs-are-good-for-everything-should-we-all-be-on-them). There were  many fascinating points, many highly relevant to something I'm currently thinking and writing about. I wanted to go back and review the content, but instead of re-listening to the whole thing, I wanted to read a transcript. I can skim quicker than trying to find specific areas of the audio podcast. 

I thought, surely there's some software out there for this, and then the next thought came: Could I actually build this myself, with the help of an AI? (It is, after all, the era of [Vibe Coding](https://en.wikipedia.org/wiki/Vibe_coding))

My general sense was that it should be possible. Most podcast players get their audio from an open, free feed, which means means there is a free audio file of a podcast episode somewhere on the internet that podcast players find and pipe to your ears. And I knew that with AI, converting audio to text is now a pretty straightforward task. 

My goal was to get Claude’s help to build a script that would do this work for me.

The plan was simple:

1. Find the audio file for a podcast episode I listened to.
    
2. Download the audio file.
    
3. Feed it into an AI model that’s good at transcription.
    
4. Get a text transcript I could read.
    

### Unfurling my noob credentials (Warning: may be painful to read if you're a programmer)

Now, I'm **not** a developer. My technical knowledge is, at best, superficial. I know what Python is, I've seen code developed by others and learnt to modify a bit through the use of an application like VSCode (VS Code is a software that lets you write and run scripts). I also know that VSCode has a "Terminal" part where I can access a python script on my computer and run it. This can also be done on the Terminal of a mac. 

This might sound painfully naive to anyone who codes, but I'm writing this for people who know as much as I do—or even less. I also had a vague memory of having installed Python 3 on my computer at some point.

So, with VS Code and Python 3 on my machine, and Claude ready to answer all my questions, I set out to see what would happen.

Of course. I'll take that next block of text and rephrase it while maintaining the same style. I'll keep the direct, personal tone and the sense of discovery you described.


First, a quick summary of what I accomplished:

-  I created a script to find and download a specific podcast episode I was interested in, saving it as an MP3 file on my computer.
- Then, I used another script to take that MP3 file and transcribe it into text. This involved figuring out how to run an AI model—specifically, a local version of OpenAI's Whisper—right on my own machine.

As I started to see what was possible, my aspirations grew. I quickly realized that simply getting one episode wasn't enough. It became obvious that the script shouldn't be limited to just one podcast; it needed to be able to download _any_ podcast episode I wanted.

This led to a new set of challenges and goals:

- I needed a way to search for and find the correct podcast "feed" on the internet, which can be surprisingly tricky since many podcasts have the same or similar names.
    
- The script also needed to be able to search within that podcast feed for the exact episode I wanted—whether by episode number, guest name, or topic.