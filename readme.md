# Mobile Suits in the Black

This is a playset for [_Scum and
Villainy_](https://www.evilhat.com/home/scum-and-villainy/) by Stras Acimov and
John LeBoeuf-Little, published by Evil Hat Games.

It adds or replaces game elements to make the core _SaV_ engine work for playing
a game set in the Gundam franchise's early Universal Century.

## Contributing

Please do! I'm making this because I want to some day play it, and I would love
for others to enjoy it too!

If you're comfortable using git and github, feel free to fork and make pull
requests. The only requirement is that you have a [Hugo](https://gohugo.io)
binary of version 0.42.1 or later. I'd also ask that you respect line-length as
much as possible. The project uses Vim's default line-length of ~80 characters,
but you should be able to make any editor auto-insert linebreaks. Having text
hard break like this makes tracking changes a lot easier for git.

To clone the repo, make sure you get the theme submodule:

```bash
git clone https://github.com/flyinggrizzly/mobile-suits-in-the-black.git \
  --recurse-submodules
```

If you're not comfortable using git or Hugo or whatever else, that's fine! You can open an issue
on the Github repo and I'll get to it as soon as I can.

### Things to be aware of if you're working with Hugo

- footnotes (which should be avoided if possible), have to be on a single line
- frontmatter should be in JSON format (there are archetypes set up for
  playbooks and mobile suits currently), and if you've got a long entry, it also
  needs to be on a single line


