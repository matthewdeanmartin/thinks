# thinks
Minimalist Social Media Experiment...on Github...alternative to Twitter in case it goes sour

To read what I think
[Thinks Feed](thinks.md)

I haven't worked out follow, aggregate, re-think, etc yet. Github's interface on its own isn't actually a replacement for twitter.

Prior Art
---
- [John Carmacks Plan files](https://github.com/ESWAT/john-carmack-plan-archive)
- [Hanselman's Ask Me Anything Repo](https://github.com/shanselman/ama)

How to start your own
---
- Fork this to participate in a conversation with me, but you'll want to start from a clean repo & the minimal artifacts
- I'll add a link to the 'starter kit' here as soon as I make one.

Social Features of a Git Repo
---
- Follow my account [mattthewdeanmartin](https://github.com/matthewdeanmartin)
- Watch this repo [watch](https://github.com/matthewdeanmartin/thinks).
- Star this repo [watch](https://github.com/matthewdeanmartin/thinks)
- Your Github notification feed now plays some of the role of the twitter newsfeed, but it will not have the stream of commits from all the `thinks` repos you follow

Social Rules
---
- Twitter was successful because you had to build a following, a chore that created a barrier to entry that just happened to filter out people who weren't good at creating content and interacting with others. The difficulty of using Git and Github is the same sort of social filter.
- Twitter also forced people to provide an abstract (that summary paragraph on academic articles) for what ever they were thinking about. But twitter, outside of tweet storms and offsite links never provided a way to write the long form.
- I think some of these rules could be self enforced with `pre-commit` rules, that would check to make sure that a `think` is a limited chunk of text
- Also, git comments are limited to 72 characters, which is too short for English, but sort of works for this purpose.

Conversations
---
- Comment on a commit. Same as reply to a tweet. You can like a reply to a commit comment, but not the original commit.
- Open an Issue. Same a mention, `@so_and_so what's up?`. I think this is also where blog posts would go.
- Fork and open a pull request. This probably would be best for community editing (fixing spelling, etc). This will let someone else add to the commit stream, so you really would need to read it with `blame` annotation for anything to make sense. Also if anyone edits someone else's text, even blame will confuse the conversation.

Actions
---
- The developer oriented UI isn't going to be the best UI, so naturally we'd want to compile the text to a static website for reading and aggregating content. It would have links back to the regular github website for the interaction/replies/etc.




