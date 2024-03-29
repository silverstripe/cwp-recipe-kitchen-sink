# DEPRECATED

This package is no longer in-use. It has been superseded by [`silverstripe/recipe-kitchen-sink`](https://github.com/silverstripe/recipe-kitchen-sink).

## CWP kitchen sink recipe

[![Build Status](https://travis-ci.com/silverstripe/cwp-recipe-kitchen-sink.svg?branch=2)](https://travis-ci.com/silverstripe/cwp-recipe-kitchen-sink)

The kitchen sink is an internal recipe used for testing full CWP feature sets, including optional and suggested
modules.

## Get started

You can create a project using Composer:

```
composer create-project cwp/cwp-recipe-kitchen-sink ./cwp2-sink ^2
```

## More information

See the [recipe plugin](https://github.com/silverstripe/recipe-plugin) page for instructions on how
SilverStripe recipes work.

## Troubleshooting

### Page and PageController parent classes

When installing the CWP kitchen sink, your project Page and PageController subclasses may be set to extend
SiteTree and ContentController. This is [only an issue](https://github.com/silverstripe/cwp-recipe-kitchen-sink/issues/30)
with the kitchen sink recipe, and requires you to manually change the parent classes to CWP's BasePage and
BasePageController.
