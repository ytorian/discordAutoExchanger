
# How to make an autoexchange bot

1. Think about the commands a bot like this would need, some are:
- Balance
- Removing / adding balance for server owner / admins
- Ticket system
2. Think about commands you could add to the bot to make it a bit nicer.
- Games (coinflip, rock paper scissors)
- Leaderboard
3. Think of how you could make the ticket system and let users deposit and withdraw
I did this by using:
- Coinbase for withdrawing
- Cashapp for depositing
- Buttons for letting users enter their address / cashapp receipt
How do you do that?
-
For cashapp you will need to do some basic web scripting, the base url for web receipts is : https://cash.app/payments/{id}/receipt?utm_source=activity-item

now i wont spoil how to do it ofcourse, but that page is loaded via js and thus hard to go and web scrape from and didnt i say some basic webscraping?? Well, try to look in the network tab (via inspecting the page) and reloading the page to see what request (get request) is used to retrieve the data. If you have figured it out, send a request to that url, and try to change the id depending on what id your user gives you via the bot.

Coinbase works via their api, this is pretty straight forward and you can look at it via:
https://docs.cloud.coinbase.com/sign-in-with-coinbase/docs/welcome
are there other options to interact with wallets and crypto? ofcourse, i chose coinbase as i liked the simplicity. however you might like something else. You can do a quick search on the internet and figure out what works best for you

Buttons are basic interaction objects, learn more about those here: https://guide.pycord.dev/interactions/ui-components/buttons (this is pycord, you might use something different)


All the other stuff around it is something for you to figure out ;) .

Why am i doing this?
-
Recently the source code of the bot i made that does this has been obtained by an individual who is now reselling it. Since then i have asked myself if i should throw the source online or a tutorial like this. I have decided for the tutorial due to me finding it usefull for others to learn how to code if you want bots like this. You will most likely be able to buy the source in a few hours if you are looking hard for it. But if you want to develop bots or become a developer yourself, dont underestimate the power of doing stuff yourself. you will learn way more!

Don't want to go through all this / just looking to purchase it?
-
You can always purchase it via contacting me on ytorianv1001 on discord. Moreover, I am working a new version of this bot (with alot of upgrades) which is publicly available to be added to your discord server. to check it out go to: https://discord.gg/swappy
