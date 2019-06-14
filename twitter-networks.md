## Options for Twitter Networks

# Streaming Twitter via Gephi (streaming only, aka drinking from the firehose)

1. import the TwitterStreamingImporter plugin for Gephi (Tools -> Plugins -> Available Plugins, listed under Import category) and restart Gephi
2. sign up for Twitter API credentials via Twitter website
3. in the Gephi Streaming Importer window (find via Window -> Gephi Streaming Importer) click the "Credentials" button and set your credentials from Twitter
4. use the add and delete buttons to add search queries, or save/load query files for repeated search
5. choose how you want the network to be constructed (full network, user-to-user network, hashtag-to-hashtag network, etc.)
6. click "Connect" button and let run!
7. click "Disconnect" button to stop the "drinking from the firehose" of Twitter before you save/quit Gephi/computer falls asleep
8. visualize/analyze away!

# Collect Tweets Over Time via TAGS (repeated uses of the free 7-day query to the archive)

1. go to www.github.com/jmotis/twitter-networks and download (or fork) the repository
2. for the totally manual workflow, follow the instructions in the Word document
3. follow the instructions in the Word document to set up TAGS and set-up a recurring query
4. let it run for however long (days, months, years) you want, up to 18,000 tweets at which point Google Sheets gets cranky
4. export your archive sheet
5. run the code! most of the code is for TAGS 6.0, but you've probably downloaded 6.1, which only works right now with networkCreation17.py
    1. if you know how to run python code, you're good! it expects the csv to be put in the same folder as the code, but you can tweak that if you want
    2. if you are not familiar with python code, never fear! here's what to do (for Mac users)
        1. put networkCreation17.py in your Home folder (reached by, in the Finder, choosing the Go menu and finding Home in the dropdown) and leave it there
        2. temporarily put the TAGS archive csv in the Home folder as well
        3. open Terminal (the application)
        4. type (without the quotes) "python networkCreation17.py" and hit enter
        5. when prompted, type the name of the csv
        6. quit Terminal
        7. move the TAGS archive csv and new edge list csv to wherever you want them permanently stored.
    3. debugging
        1. if you get an error message, you may not have Python installed or have an old version of Python. Go to www.github.com/ComputeCanada/dhsi-coding-fundamentals-2019 and follow the instructions there to install Anaconda, which will also install Python 3.x for you
        2. if you are on a Windows machine, I think you need to put it in your C: Drive, but anyone who programs on your campus should be able to help you find whatever root directory opens in the console. You do not have a built-in console like Macs, but Anaconda (above) which installs Python 3.x should also install a console program you can use.

# Collect Tweets Via Programming (streaming and/or various ways of querying the archive)

1. fork or clone or download www.github.com/ComputeCanada/dhsi-coding-fundamentals-2019
2. in the Jupyter Notebooks folder, there is a notebook on Twitter Scraping for Researchers
3. sign up for Twitter API credentials via Twitter website and have at it!