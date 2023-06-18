# Ghost Buses Blog

Welcome to the blog for the Ghost Buses Breakout Group at ChiHackNight. If you have an idea for a post, new features, or other improvements, please submit a pull request.

## Setup

You will need to have Ruby and Jekyll installed on your machine. Here are installation instructions for [Jekyll](https://jekyllrb.com/docs/installation/) and [Ruby](https://www.ruby-lang.org/en/documentation/installation/). You can also use [rvm](https://www.ruby-lang.org/en/documentation/installation/) to manage Ruby versions.

Once installed, you can run
```
git clone https://github.com/chihacknight/chn-ghost-buses-blog.git
cd chn-ghost-buses-blog
rvm install ruby-3.0.2
bundle install
```
To run locally, use
`bundle exec jekyll serve`

The site will be available at `http://localhost:4000`.

### Docker
If you prefer to use Docker, you can run
```code
docker run --rm --label=jekyll --volume="$PWD:/srv/jekyll" -it -p 4000:4000 jekyll/jekyll export JEKYLL_VERSION=4.2 | bundle install | jekyll serve -w
```

More information on running Docker with Jekyll can be found [here](https://ddewaele.github.io/running-jekyll-in-docker/).


## Posts
To write a post, create a file in the `_posts` directory with the format `YYYY-MM-DD-title.md`, where `YYYY` is the four digit year, and `MM` and `DD` are the two digit month and day respectively. 

To write a draft post, create a `_drafts` directory in the site root and create a file without a date in the file name. To preview your site with drafts, use `bundle exec jekyll serve --drafts`.

See [here](https://jekyllrb.com/docs/posts/) for more information about formatting blog posts. 



