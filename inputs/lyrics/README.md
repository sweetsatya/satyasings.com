## A process of adding and modifying songs

- Write lyrics, translation, credits and background for each song on Google docs
- Copy the above to `.md` file for each song in this directory.
  - The song has a title and subheadings (e.g., lyrics, translation)
  - An empty line separates verses
- Update the "tracklist" in `template.html` - this shows up as the album list on the website
  - The title of the `.md` file should match the heading of the song, not the name of the .md document
- Type `make` which [builds](../../Makefile) `lyrics.html` and `index.html`
  - Run every time you make changes to content or style BEFORE committing changes to catch errors
  - `lyrics.html` is produced from the txt files via [python script](../../scripts/generate_lyrics.py)
  - `index.html` is the output file: songs flow from `lyrics.html`, album listing from `template.html`