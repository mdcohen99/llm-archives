# llm-archives

### Instructions

Click the "Use this template" button for this repository and choose "Create a new repository". You can give it the same name (llm-archives).

Once it's ready, go to [Groq](https://console.groq.com/keys) and follow the directions to get an API key. You'll need to login (or create an account if you don't have one).

Copy the API key value and then click on the Settings of your GitHub repository and click on "Secrets and variables" on the left side, then choose "Codespaces"

Click the green "New Repository Secret" button and paste your API Key into the "Secret" box, then put GROQ_API_KEY in the Name box above it. Click "Add Secret" and click on the name of the repository to return to the main page.

From there, click the green "Code" button and create a new Codespace in the Codespaces tab.

In the Terminal type the following: pip install requests groq and hit enter.

Then type: python get_stories.py

You should see a file called cns_maryland_posts.json appear. Let's look at it. It contains some details of the past 10 CNS stories.

Back in the Terminal, type: python entity_extraction.py and watch the output.

### Evaluation for JOUR389W

This seems generally pretty solid in terms of the model's ability to parse out the important information. It generally got all the locations right and people's names and such. In the sake of using AI to read articles like this, there may not be a ton of utility out of these pieces of information. 

To me, I see the utility more so in basically using it as a more accurate version of using "control F" in a large set of records. If, for example, I was writing this story about Tommy Tuberville's residency, I may have large sets of documents regarding his information/address history/voting history and it may be too much to be able to read and control F isn't always fully reliable, especially in PDFs. This seems like a much better method of looking for something in a large set of documents if, say, I was trying to find Tuberville's name amidst the documents to prove he was connected to x or y. 

In terms of actual stories, if we saw a name we weren't expecting come up in this story, let's just say Nick Saban for the sake of another football connection who likes to yap a lot too, we could then try to extrapolate further. What other stories does Nick Saban show up? Is he showing up frequently with Tuberville (doubt it, Saban is good friends with Joe Manchin and is a closeted democrat in republican central)? We can look for trends in terms of who is showing up also with what locations and lead us to further questions that could lead to more interesting stories whether it be trend stories, investigations or just simply a good brainstorming sessions about important people. 
