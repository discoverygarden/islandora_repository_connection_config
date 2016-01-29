# Islandora Repository Connection Configuration

## Introduction

Tuque has a number of parameters which are not otherwise exposed... So let's expose them.

## Requirements

This module requires the following modules/libraries:

* [Islandora](https://github.com/islandora/islandora)
* [Tuque](https://github.com/islandora/tuque)

## Installation

Install as usual, see [this](https://drupal.org/documentation/install/modules-themes/modules-7) for further information.

## Usage

We add another vertical tab to `admin/islandora/configure`, called "Tuque connection config", to expose connection parameters.

There are a couple excluded from our form, such as:
* `HttpConnection::$sslVersion`, corresponding to `CURLOPT_SSLVERSION` (which presently has a big note in the PHP manual pages recommending the default)
* `HttpConnection::$url`, since it is URL provided in the core config
* `HttpConnection::$username` and `HttpConnection::$password`, since they are handled in our usual instantiation routine (set with the current user creds)

## Troubleshooting/Issues

Having problems or solved a problem? Contact [discoverygarden](http://support.discoverygarden.ca).

## Maintainers/Sponsors

Current maintainers:

* [discoverygarden](http://www.discoverygarden.ca)

## Development

If you would like to contribute to this module, please check out our helpful
[Documentation for Developers](https://github.com/Islandora/islandora/wiki#wiki-documentation-for-developers)
info, [Developers](http://islandora.ca/developers) section on Islandora.ca and
contact [discoverygarden](http://support.discoverygarden.ca).

## License

[GPLv3](http://www.gnu.org/licenses/gpl-3.0.txt)
