### Feed generator
- Turn `thinks.md` into a html file
- Links to the commit comments

### Simulate Followers
- Querying every single FRIENDS.authors file and seeing if they follow you, is not going to scale.
- Compile a list of everyone that has *interacted* with you instead. Misses lurkers, but easy to scale.

### CHANGELOG support
- Either changelog for actual app changes or life changes/thoughts
- Changelog repurposed for general purposes

### Plain text support
- File format is just cr, or lf or crlf delimited text

### Multiple 'persona' support
- In twitter this is done with multiple accounts
- Maybe do this in multiple branches? multiple files?

### Twitter import
- Turn twitter into month by month thinks.md files

### Thinks client
- Allow for adding a think in one step, rather than editing the md file & commit & push
- Allow for edit of FRIENDS, FOLLOWS files (in format of AUTHORS)
- Allow for quick edit of FRIENDS.authors file
- 
### Aggregate
- Follow CHANGELOG, think.md or arbitrary plaintext
- Follow RSS
- Follow Twitter for people who aren't with the new way (needs API key)
