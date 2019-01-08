# Islandora Repository Connection Configuration

## Introduction

Tuque has a number of parameters which are not otherwise exposed... So let's
expose them.

## Requirements

While it does not strictly require them, this module's purpose is to augment:

* [Islandora](https://github.com/discoverygarden/islandora)
* [Tuque](https://github.com/islandora/tuque)

## Installation

Install as
[usual](https://www.drupal.org/docs/8/extending-drupal-8/installing-drupal-8-modules).

## Usage

We add another vertical tab to `admin/config/islandora/configure`, called
"Tuque connection config", to expose connection parameters.

There are a couple excluded from our form, such as:
* `HttpConnection::$sslVersion`, corresponding to `CURLOPT_SSLVERSION` (which
presently has a big note in the PHP manual pages recommending the default)
* `HttpConnection::$url`, since it is URL provided in the core config
* `HttpConnection::$username` and `HttpConnection::$password`, since they are
handled in our usual instantiation routine (set with the current user creds)

## Troubleshooting/Issues

Having problems or solved a problem? Contact
[discoverygarden](http://support.discoverygarden.ca).

## Maintainers/Sponsors

Current maintainers:

* [discoverygarden](http://www.discoverygarden.ca)

## Development

If you would like to contribute to this module, please check out the helpful
[Documentation](https://github.com/Islandora/islandora/wiki#wiki-documentation-for-developers),
[Developers](http://islandora.ca/developers) section on Islandora.ca and create
an issue, pull request and or contact
[discoverygarden](http://support.discoverygarden.ca).

## License

[GPLv3](http://www.gnu.org/licenses/gpl-3.0.txt)
