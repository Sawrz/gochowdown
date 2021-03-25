# Gourmet Secrets

A theme for [Hugo](https://gohugo.io/) forked from the [GoChowdown](https://github.com/seanlane/gochowdown) Theme, build on the [Chowdown](https://github.com/clarklab/chowdown) theme for Jekyll.

<p align="center">
  <img src="https://gitlab.com/sawrz/gourmet-secrets/-/raw/master/images/screenshot.png" />
</p>

## Quick Start

0. Install Hugo with your favorite package manager, or follow their [Installation Guide](https://gohugo.io/getting-started/installing/)
    - Note that the _extended_ version of Hugo is required since this theme needs SCSS support. At the time of writing, this is the version found by installing via [HomeBrew](https://github.com/Homebrew/homebrew-core/blob/master/Formula/hugo.rb) and the [Arch User Repository](https://www.archlinux.org/packages/community/x86_64/hugo/). If that isn't the case for your package manager, install using `$ go install --tags extended` as documented in the Hugo Install Docs.
1. Add the repository into your Hugo Project repository as a submodule, `https://github.com/Sawrz/gourmet-secrets themes/gourmet-secrets`.
2. Configure your `config.toml` or `config.yaml`.
3. Build your site with `hugo server` and see the result at `http://localhost:1313/`.

## Using this theme

Like [GoChowdown](https://github.com/seanlane/gochowdown), this theme adds two sections, recipes and components. The primary section you'll want to use is the recipes, as they form the panel listing on the front page and most of the content. The components section is for recipes that form subcomponents of a recipe, allowing for a recipe to call on several components and recipes to reuse the same component if desired.

### Add a new recipe draft

1. Navigate to the root directory of your website folder within a terminal
2. Type `hugo new --kind recipe-bundle recipes/name-of-your-new-recipe-here`, replacing `name-of-your-new-recipe-here` with the name of your recipe
  - Note that the default template (archetype in Hugo vernacular) will replace the hyphens in the provided name with spaces as the title and capitalize each word's first letter. For example, if I were to enter the command `hugo new --kind recipe-bundle recipes/hot-dog`, I would find a new folder at `content/recipes/hot-dog`, and the title within the `index.md` file in that folder would be `Hot Dog`.

### Add a new recipe with components

Like above, instead of adding the recipes to the `content/recipes` directory, add the individual components to the `content/components` directory. Then add a new recipe as you normally would, and replace the instructions list with a components list, using the title (aka name) of the recipe, and modify the directions section as needed.

## Disclaimer

This theme is sort of a Frankenstein theme based on [GoChowdown](https://github.com/seanlane/gochowdown), [Docsy](https://github.com/google/docsy) and my own work. I'm no web developer by trade, nor I intend to become one. I did my best to keep everything as consistent as possible, but if you find something that can be improved, let me know or issue a PR (preferred).

Since I built this theme for personal purposes only, SEO was none of my priorities. If you would like to optimize this theme, feel free to join, or issue a PR.

## Credits

- [GoChowdown](https://github.com/seanlane/gochowdown) (forked from)
- [Docsy](https://github.com/google/docsy) ("borrowed"/rewrote huge chunks of code")
- [Chowdown](https://github.com/clarklab/chowdown) (base for GoChowDown)
- [Hugo](https://gohugo.io/) (wouldn't be possibile without it)

## License

Code is licensed under the [MIT license](https://github.com/Sawrz/gourmet-secrets).

