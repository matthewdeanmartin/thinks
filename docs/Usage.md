# Main workflows

This is mostly not implemented, except features native to Github!

My design goal is to see if each workflow:

- could in theory be done with the Github web interface.
- could interact with `thinks` unaware formats, e.g. plain text, rss, twitter, etc
- use microformats (broadly described) when possible, such as CHANGELOG and AUTHORS
- has twitter refuge features such as "import all data from twitter" and "mirror to twitter"

# Reading what people think

Run app that queries your FRIENDS.authors file and generates a pretty HTML file. This file would not be uploaded
to github.

```bash
pipenv shell
python -m thinks -generate-feed FRIENDS.authors
open "newfeed.html"
```

# Writing things

Several options

- Edit your thinks.md file using Github's web interface, or your favor other way.
- Edit a thinks.txt file
- Edit a CHANGELOG format file, e.g. thinks.changelog

Commit and push your thought. Ideally, the thought in the file and the commit comment are the same. When they are the
same, the git history and thinks.md file are in synchronization and you don't really need to use a static site generator
to create a thinks.html page for your audience to view your thoughts.

Github actions and Github pages will handle generating nice HTML view with the appropriate links to the commit comments
pages.

Unless you are using an app to do this in one single transaction, it is likely to not be the same. So ideally, you'd
want to use a client that edited the file and put the `think` text into the git comment, committed and pushed all at
once.

```bash
pipenv shell
python -m thinks -post "I think I should buy a boat"
```

# Following people

Several options

- Bookmark the commit history of each person you follow.
- Edit your FRIENDS.authors file using the AUTHORS file format.
- Use a tool to edit the AUTHORS file, commit, push and regenerate your newsfeed
- Use a tool to convert a twitter follow list to FRIENDS.authors format

```bash
pipenv shell
python -m thinks -follow "matthewdeanmartin (https://github.com/matthewdeanmartin/thinks/blob/main/thinks/)"
```

# Conversations
- Comments on commits and Github notifications for replies.
- Reactions on your own `thinks` log for "replying" to people who are posting a format that doesn't support replies.

When doing Github native comments, everyone gets a notification. If you do a "reaction" to someone, there won't be a
way for them to realize that you are talking to them. I guess you could use the github source code search to see
if any source code references your name.

```bash
pipenv shell
python -m thinks -reply "<url to think>" "cool!"
```


```bash
pipenv shell
python -m thinks -follow "matthewdeanmartin (https://github.com/matthewdeanmartin/thinks/issues/)"
```