## Jetpack Smooth Generator

Inspired by [WooCommerce Smooth Generator](https://github.com/woocommerce/wc-smooth-generator), **Jetpack Smooth Generator** creates dummy content via the command line interface providing the site with different combinations of posts and Jetpack settings. 

**Currently not functional**.


## How does this work

For content generation, this plugin downloads content from a _mother site_ where content has been previously created. 

Some plugins generate content on the fly but having a mother site where the content gets generated by hand allows Jetpack developers to find hard-to-reproduce conditions on other sites where Jetpack would probably error unless a particular combination of content and settings is set in place.

**Jetpack Smooth Generator** allows us to test different combinations of widgets, shortcodes, images, or Gutenberg blocks on posts and perceive the behaviour of Jetpack in a simulation of _the wild_

## Example usage

Generate 12 posts

```sh
wp jetpack generate posts 12
```

Generate random combination of Jetpack settings

```sh
wp jetpack generate settings
```

## Development

The `features` directory contains a file for each subcommand added on top of `wp jetpack generate`. 


## License

GPL2
