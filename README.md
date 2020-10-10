
## Usage

You can edit `_config.yml` file to customize your blog. You can change things such as the name of the blog, the author, the appearance of the theme (light, dark or auto), how dates are formatted, etc. Customizable fields should be straightforward to understand. Still, `_config.yml` contains some comments to help you understand what each field does.

For further customization (e.g. layout, CSS) see the [official Jekyll's documentation](https://jekyllrb.com/docs/themes/#overriding-theme-defaults) on customizing gem-based themes.

### Customize the menu

In order to add/edit/delete entries from the main menu, you have to edit the `menu.yml` file inside `_data` folder. Through that file you can define the structure of the menu. Take a look at the default configuration to get an idea of how it works and read on for a more comprehensive explanation.

The `menu.yml` file accepts the following fields:

- `entries` define a new unordered list that will contain menu entries
- each entry is marked by a `-` at the beginning of the line
- each entry has the following attributes:
    - `title`, which defines the text to render for that menu entry
    - `url`, which can either be a URL or `false`. If it is `false`, the entry will be rendered as plain text; otherwise the entry will be rendered as a link pointing to the specified URL. Note that the URL can either be relative or absolute.
    - `post_list`, which can be `true` or `false`. If it is true, the entry will have all posts in the site as subentries. This is used to render your post list.
    - `entries`, yes, you can have entries inside entries. In this way you can create nested sublists!

### Pro tips

#### Dark mode for images

This theme provides dark mode by inverting all colors of light mode throught the CSS `invert()` function. This approach would also invert the color of all images, but, since this is not the behaviour one would expect, images are not inverted by default.

However, if you would like to force the color inversion on a specific image you can do so by applying `class="ioda"` to that image ("ioda" stands for "invert on dark appearance"). See the image in the [overview post](https://github.com/riggraz/no-style-please/blob/master/_posts/2020-07-07-overview-post.md) for an example of this approach. Note that color inversion will take place only when the theme has dark appearance!

For example, if you have a black and white image it could make sense to invert it in dark mode. On the other hand, a colorful image will probably look bad if inverted.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

