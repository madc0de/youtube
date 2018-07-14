# YouTube API v3 PHP Wrapper & YouTube Downloader

A basic PHP wrapper for the Youtube Data API v3 ( Non-OAuth ). Designed to let devs easily fetch public data (Video & Channel) from Youtube. No 3rd party dependancy. The reason of returning the ARRAY response directly is to keep it simple.

Some parameters are missing in this library, because I don't need them at this point, if you desire a particular feature please file an issue here :smile:

## Requirements

* PHP >=5.3
* CURL extension in PHP

## Install

Run the following command in your command line shell in your php project

```
composer require madcodez/youtube
```

## Usage

### Example usage of Searching :

```php
<?php
require 'vendor/autoload.php';

$youtube = new Madcodez\YouTube\YouTube('* Your API key here *');

$seach = $youtube->search('Web Development', '10', $pageToken);

print_r($search);
```

### Example usage of video info :

```php
<?php

require 'vendor/autoload.php';

$youtube = new Madcodez\YouTube\YouTube('* Your API key here *');

$video = $youtube->video('rie-hPVJ7Sw');

print_r($video);
```

## Format of returned data

The returnd data is a PHP Array

## Youtube Data API v3

* [Obtain API key from Google API Console](https://code.google.com/apis/console)

## Contact

For bugs, complain and suggestions please [file an Issue here](https://github.com/madcode-git/youtube/issues) or send email to madcode.git@gmail.com :smile:

## License

This library is licensed under the [MIT License](http://opensource.org/licenses/MIT).
