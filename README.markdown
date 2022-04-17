# ACID THEME REGISTRY

## About :books:

This is the official repository for the source of Acid's official theme registry! You can find out more about ***Acid*** [here](https://github.com/iamtheblackunicorn/acid).

## Usage :hammer:

I'm assuming that you have ***Acid's*** latest version installed and available from the command line!
If you do, run these commands:

- 1.) Get the source code:

```bash
$ git clone https://github.com/iamtheblackunicorn/acid-themes
```

- 2.) Get the source code:

```bash
$ cd acid-themes
```

- 3.) Compile the website.

```bash
$ acid-rs --build .
```

This should produce a bunch of HTML and CSS files in a child directory called `build`.

## Contributing :scroll:

### Requirements

I'm assuming you have [***Acid***](https://github.com/iamtheblackunicorn/acid) and Git installed on your system and both of them available from the command line.

### Steps

This is the most important part!
If you've been using [***Acid***](https://github.com/iamtheblackunicorn/acid) and you've developed your own theme live on GitHub, you can add your theme like this:

- 1.) Fork this repository on GitHub.
- 2.) Clone the repository to your machine with the following command.
  ```bash
  $ git clone https://github.com/iamtheblackunicorn/acid-themes
  ```
- 3.) Create a file in the `posts` directory, called `YYYY-MM-DD-Your-Theme-Name.markdown`, where `YYYY` represents the year, `MM` represents the month, `DD` represents the day, and `Your-Theme-Name` represents the name of your theme sepearated by dashes.
- 4.) Put the following into this file:
  ```markdown
  ---
  title:Acid Tripping
  layout:post
  repo:iamtheblackunicorn/acid-tripping
  banner:assets/images/acid-tripping.png
  description:Acid's first theme!
  ---

  ## Some Info Heading
  Some info about your theme.
  ```
  - `title`: The name of your theme!
  - `layout`: Fill this with `post`.
  - `repo`: Where is your theme? Fill this with `yourusername/yourthemerepo`, where `yourusername` represents your GitHub username and `yourthemerepo` represents the name of the repo where you keep your Acid theme.
  - `banner`: The local path to your theme. This repository has a an `assets` folder with an `images` folder. Put the screenshot of your theme there. Name it thusly: `your-theme.png`, where `your-theme` is the name of your theme separated by dashes.
  - `description`: A short description of your theme.
  Fill the rest of this file with whatever info you'd like to add.
- 5.) Test that this site builds by running `acid-rs -b .` in the root of this Acid site and subsequently, check everything looks how it is supposed to, by running `acid-rs -s .`.
- 6.) Commit and push your changes.
- 7.) File a Pull Request!
