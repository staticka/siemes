# Siemes

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]][link-license]
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Total Downloads][ico-downloads]][link-downloads]

A easy-to-use flat file content management system based on [Staticka](https://staticka.github.io).

## Install

Via [Composer](https://getcomposer.org)

``` bash
$ composer global require staticka/siemes
```

## Usage

Create a new file named `hello-world.md`:

**hello-world.md**

```
# Hello World!

This is my first post that is built with Siemes by Staticka.
```

Then run the `siemes build` command to build the files:

``` bash
$ siemes build
```

To see the output, open `build/hello-world/index.html` in a web browser.

**build/hello-world/index.html**

``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Hello World</title>
</head>
<body>
  <h1>Hello World</h1>
  <p>This is my first post that is built with Siemes by Staticka.</p>
</body>
</html>
```

### Options

* `--source` - Location of the content files

``` bash
$ siemes build --source="pages"
```

Looks for content files from the `page` directory.

* `--output` - Path for generated HTML

``` bash
$ siemes build --output="output"
```

Puts all the compiled content files to the `output` directory.

* `--website` - Custom Website instance

``` bash
$ siemes build --website="Acme.php"
```

Uses the `Acme.php` as the `Siemes\Website` instance.

## Change log

Please see [CHANGELOG][link-changelog] for more information what has changed recently.

## Testing

``` bash
$ composer test
```

## Security

If you discover any security related issues, please email rougingutib@gmail.com instead of using the issue tracker.

## Credits

- [Rougin Royce Gutib][link-author]
- [All contributors][link-contributors]

## License

The MIT License (MIT). Please see [LICENSE][link-license] for more information.

[ico-version]: https://img.shields.io/packagist/v/staticka/siemes.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/staticka/siemes/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/staticka/siemes.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/staticka/siemes.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/staticka/siemes.svg?style=flat-square

[link-author]: https://rougin.github.io
[link-changelog]: https://github.com/staticka/siemes/blob/master/CHANGELOG.md
[link-code-quality]: https://scrutinizer-ci.com/g/staticka/siemes
[link-contributors]: https://github.com/staticka/siemes/contributors
[link-downloads]: https://packagist.org/packages/staticka/siemes
[link-license]: https://github.com/staticka/siemes/blob/master/LICENSE.md
[link-packagist]: https://packagist.org/packages/staticka/siemes
[link-scrutinizer]: https://scrutinizer-ci.com/g/staticka/siemes/code-structure
[link-travis]: https://travis-ci.org/staticka/siemes