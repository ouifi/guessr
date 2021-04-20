- [Guessr](#guessr)
- [Getting Started](#getting-started)
- [Technologies Used](#technologies-used)
- [Feature/Contribution Ideas](#featurecontribution-ideas)

<p align="center">
    <img id="image" src="./logo.png" width="20%">
</p>

# Guessr
A fun small web app for Reddit

# Getting Started
See the client/ and server/ Readme's to get started running each.

# Technologies Used
Frontend:
- React
- TypeScript
- React-Bootstrap
- Bootstrap
- HTML5/CSS3

Backend:
- Fastify
- Reddit API

# Feature/Contribution Ideas

These are some ideas for features to add that I considered unneccessary for getting this project off the ground. PR's are welcome!

- NSFW allowed (yes/no)
- Better submission <=> correct answer comparison. Currently this just uses case-insensitive string comparison. I was thinking using something like fast/est-levenshtein to make small typos forgivable
- Actual leaderboards. IDK. This would require some kind of data store to back the server. Im not super interested in this idea, but someone can fork the repo if they want to add it. 
- User OAuth permissions. Currently this app uses a couple of reddit bot accounts I created, and it will rotate/load balance between the two bot accounts to stay within Reddit usage rates. Having the option for a user to sign in via OAuth on their own account would mean they could play to their hearts' content. This may be a good idea for someone more experienced in OAuth flows to implement. 
- New Game Modes. I have ideas for 2 game modes, challenge and time trial. In challenge mode, you start with only having one post presented, then you continue to get more until you are able to get the sub reddit or give up. In time trial, you have 2 minutes to play as fast as you want, with no rules, trying to get as many subreddits as possible until the timer hits 0. 