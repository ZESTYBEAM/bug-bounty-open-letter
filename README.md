# Bug Bounties: An Open Letter to The Decentral Games Community

## The Infinite Chips Glitch

Sers,

As most of you in the Decentral Games community are aware by now, in the
months of May and June 2023, ICE Poker had a rather nasty chip exploit.
How nasty? Let's walk through the most condensed steps to reproduce it:

1. Walk up to an empty table and click on the cards.
2. Buy in for the desired amount, between 400-3000.
3. Back away from the table and count to 3.

Using this method, it was possible to glitch in an extra 400 to 3000 
chips. Not convinced? Here's raw video (Courtesy of Donboss) showing off 
the exploit:

[Buying in 3k chips at a time](https://youtu.be/BcMvfjoZ4IQ)

[Buying in 400 at a time](https://youtu.be/XhOH7KeLJOA)


## Glitch Hunting and Reporting

Once my merry band of friends and I noticed that the leaderboards were 
extremely off, we decided to start using Diamond Hands City as a test bed 
to try to reproduce the chip exploit. This allowed us to iterate rapidly, 
since we didn't have to deal with table cooldowns. It took about a week, 
but Katma had the first breakthrough with a method that involved leaving 
an empty table, going to a populated table, and refreshing. Others, as I 
found out later, had stumbled upon similar methods and reported them. 
About 10 minutes after Katma posted about the longer method in a group DM, 
Donboss figured out the magic that's on display in the videos.

With this information in hand, there was a debate over how to proceed. Two 
tickets later and ultimately, we disclosed the exploit to the Decentral 
Games team, even after being told that since the bug was known to the 
team, it wasn't eligible for a bug bounty. The debate over how to proceed 
was civil but divided, and it was ultimately Diarhea's words of wisdom 
about responsible disclosure being good for our bags that swayed us in 
favor of providing the team with all the information. Just to make this 
write-up spicier, I was originally fully in favor of NOT disclosing the 
bug unless the Decentral Games team was willing to pay out, but that has 
to do with the fact that I still fondly recall the days when anti-security 
was the most optimal approach to exploits.

I was later told in one of my tickets that the findings I presented on 
behalf of my friend group were a big help in fixing the chip exploit. 
Along the way, we were left with the impression that we may have been on 
thin ice for testing as much as we were. Thus, we didn't take this as far 
as I feel we could have, mainly in that we never did get to figure out the 
glitch that takes chips away, which may or may not be lurking in the 
codebase.

## Better Bug Bounties

As big of a fan as I am of Decentral Games, the team's current approach to 
bug bounties is not ideal, especially with the casino in play. If DG had a 
clearer rewards structure and a path for safely bug hunting without risk 
of violating the Terms of Service, severe bugs like this would get 
reported a lot faster, instead of large chunks of the playerbase 
exploiting them for over a month. This is Web3 sers, use the greed of the 
players to your advantage.

On this front, I think Decentraland has a really good [bug bounty program](https://immunefi.com/bounty/decentraland/). 
The rewards are high enough to make disclosing via the bug bounty program 
the only good option, and the rules are also very clear in what you can 
and can't do. For example, Decentraland's bug bounty program explicitly 
calls out using a testnet. Either testing on a testnet or perhaps at a 
special venue on mainnet that doesn't actually pay out ICE but nonetheless 
allows us to freely test would go a long way towards offering a safe 
harbor for people who want to make the games better.


Without clearly defined rewards and a path to testing that stays within 
the Terms of Service, the alternatives to disclosing a bug to the team 
look something like this:  
  
1. Keep it to yourself. (Non-disclosure/anti-security)
2. Drop a proof of concept and bask in the chaos. (Full disclosure)
3. Sell to a dirty owner or manager for the bag that DG will only very selectively pay out under the current system. (The "sell 0days to governments" equivalent)

These alterate outcomes are bad enough when it's just Challenge Mode at 
Stronghold/Diamond Hands City, but what if there's an exploit at Tominoya?

## Conclusion

This open letter could have been a *lot* longer. Instead, I cut it down to 
just the things that matter, and hope this will kick off a productive 
discussion on how bug bounties should be handled going forward. It's my 
opinion that the current process is vague to the point of being useless, 
and I'd love to see that change for the better. 

Old school hacker style greetz 2 Diarrhea, Donboss, Hayabusa, Katma, and PennyRich