# easy

An ultra minimalist theme for Jekyll.

## Installation

Clone or Download this Repo, and `jekyll build`.

## Development

To set up your environment to develop this theme, run `bundle install`.

To test the theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test the theme's contents. As you make modifications to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

## Usage

### Data

+ `menus.yml` - You can list down the links here that you want to display on the homepage.

### Includes

+ `archive` - Weird stuff to list down all the tags, count the number of posts under each tag, and show them on the `tags` page.

### Layouts

There are five layouts in total, you would mostly use two (unless you want to tweak the standard pages)-
+ `post` - Writing a `post`? Use this layout.
+ `page` - Need to add a page? `page` is the layout you are looking for.
+ `home` - Layout of the home` page.
+ `blog` - Layout of the \blog page.
+ `tagpage` - Layout of the \tag page.

### Color Themes

easy currently supports `light` and `dark` themes. You can set this attribute in `_config.yml` file.

### Special notes

+ When the `base_url` attribute is set to anything other than blank in `_config.yml` file, the "tag" page will break while accessing on your local machine. But don't worry, it will work just fine when deployed on GitHub Pages, etc. An easy turn-around is to leave this attribute blank when working in local, and change it back to your required base_url when pushing the changes to GitHub or anywhere else.
+ `tag` page is not created dynamically. So you'll need to add a markdown file (like tagname.md) under the tag directory and fill it with basic front-matter. This will compile into a proper html file and list all the posts under the respective tag.

## Contributing

Bug reports and pull requests are welcome at [pnin/easy](https://github.com/pnin/easy).

## License

This theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).