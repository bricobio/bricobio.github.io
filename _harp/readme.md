# Bricobio

## About

## Contributing Content

> Before getting started, please verify what's needed on Trello, or propose your own new content there.
  - [Online Content]()
  - [Blog Posts]()

> This is also the best way to get help, if you need it, when adding new content to the site!

1. To begin Locate the folder you need.
  - if you're writing a blog post:
    -   `_harp/public/en/news/`
  - if you're writing something else:
    - `_harp/public/en/{your folder}`
2. create a new `.jade` flie in this folder.
  - name it with a single word, or several-hyphenated-words
  eg: `great-event.jade` or `contact.jade`
  - no spaces in file names!
3. Copy and paste this template into your file.
4. Using [jade](http://jade-lang.com), which is shorthand for html, write your blog post.
  - please look at the [jade documentation](http://jade-lang) if you are unfamiliar with it.

  ```jade
  //- ENGLISH VERSION.
  if current.path[0] == "en"
  //- do not remove these lines
  //- Write the content below this line

    p the content here.

    img(src="/img/yourimage.png")

  //- Write the content above this line.
  //- -----------------------------------
  //- VERSION FRANÇAIS
  else if current.path[0] == "fr"
  //- Supprimez pas ces lignes
  //- Écrivez le contenu en dessous de cette ligne

    p le contenu ici

    img(src="/img/yourimage.png")

  //- Écrivez le contenu en dessus de cette ligne
  ```
5. Submit a [pull request](https://help.github.com/articles/creating-a-pull-request/), so your content can go online.

## Development

1. install node
2. `npm install -g harp`
3. Clone this repository.

  ```bash
  git clone https://github.com/bricobio/bricobio.github.io.git
  ```

4. To view changes locally:
  ```bash
  cd bricobio-website # the directory your repository is in
  harp server _harp -p 9000
  ```
  then paste this into the address bar of your browser: `localhost:9000`.

### Deploying to GitHub Pages

1. Delete `_harp/fr` directory. Make a copy of `_harp/en` and rename it `fr`.
2. Open up a terminal, enter the following commands

  ```bash
  cd bricobio-website # the root directory for your cloned git repository
  harp compile _harp/. ./
  ```

## Contributing

#### 1. Create Trello account.
- Look through the development board

#### 2. Create github account.

#### 3. Fork the repository
- Make the changes you'd like to make.
- Push your changes to your repository.

#### 4. Submit a pull request
- Our to have your changes incorporated.
