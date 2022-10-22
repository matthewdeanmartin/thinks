# thinks

Minimalist Social Media Experiment...on Github...alternative to Twitter in case it goes sour

To read what I think

- [Thinks Feed](thinks/2022-10-thinks.md)
- [Commit history](https://github.com/matthewdeanmartin/thinks/commits/main/thinks.md) (click commit hash to see
  comments on each `think`)

Unadvisedly, I'm putting my `thinks` and the support code that transforms them into friendly html & generates
a feed of people I follow all in the same repo.

General Idea
---
What if we used the features of Github to simulate Twitter?

Mostly using built in Github features

- A place to write short texts in an evergrowing markdown file.
- A place for long posts in the Issues section
- A way to reply to `thinks` via commit comments

Augmented by some microformat driven tooling

- A way to aggregate the commits to any other similar repo (repos with a text file that someone logs new activities or
  thoughts to)
    - The `thinks` file could be just lines, i.e. any CR deliminted file, so people unaware of the `thinks` format could
      be followed
    - The `thinks` file could be based on the CHANGES.md format (except it would be chronological life events and
      thoughts, not library bug fixes)
    - The `follow/friend` list could be based on the AUTHORS format
- A way to find, follow and generate static HTML views of your own and friends content.

Prior Art
---

- [John Carmacks Plan files](https://github.com/ESWAT/john-carmack-plan-archive)
- [Hanselman's Ask Me Anything Repo](https://github.com/shanselman/ama)

How to start your own
---
I'll add a link to the 'starter kit' here as soon as I make one.

I'm imagining that people would create a clean repo (don't fork this) and either manually or with a command line tool,
continually edit a small thinks.md file (or a text file, or a CHANGES file, etc)

The developer oriented UI isn't going to be the best UI, so naturally we'd want a tool to compile the text to a static
website for reading and aggregating content. It would have links back to the regular github website for the
interaction/replies/etc.

Social Rules that made Twitter Successful and could be transferred to Github
---

- Twitter was successful because you had to build a following, a chore that created a barrier to entry that just
  happened to filter out people who weren't good at creating content and interacting with others. The difficulty of
  using Git and Github is the same sort of social filter.
- Twitter also forced people to provide an abstract (that summary paragraph on academic articles) for what ever they
  were thinking about. But twitter, outside of tweet storms and offsite links never provided a way to write the long
  form.
- I think some of these rules could be self enforced with `pre-commit` rules, that would check to make sure that
  a `think` is a limited chunk of text
- Also, git comments are limited to 72 characters, which is too short for English, but sort of works for this purpose.

Conversations
---

- Comment on a commit. Same as reply to a tweet. You can like a reply to a commit comment, but not the original commit.
- Open an Issue. Same a mention, `@so_and_so what's up?`. I think this is also where blog posts would go.
- Fork and open a pull request. This probably would be best for community editing (fixing spelling, etc). This will let
  someone else add to the commit stream, so you really would need to read it with `blame` annotation for anything to
  make sense. Also if anyone edits someone else's text, even blame will confuse the conversation.
- View in a `thinks`-unaware way your conversations in the [github notifications](https://github.com/notifications)
- Also your email client becomes part of the overal experience


Docs
----

- [TODO](docs/TODO.md)
- [Usage](docs/Usage.md)
- [Analogies](docs/Analogies.md)