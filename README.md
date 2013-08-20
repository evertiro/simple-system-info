# Simple System Info v1.0.0

A simple system info class which can be dropped into a WordPress theme or plugin to provide immediate debugging info. The inclusion of several actions and filters allows extension of the class to suit your needs.

## Features ##

* Easy to use
* Easy to extend

## Thanks ##

SSI is based heavily on the awesome System Info page included in [Easy Digital Downloads](http://www.easydigitaldownloads.com).

## Getting SSI ##

SSI can be downloaded in several ways which are outlined below. Please use whichever way you are most comfortable with.

### Download as a .zip archive ###

* Dev release: [download](https://github.com/ghost1227/Simple-System-Info/archive/master.zip)

Once you have downloaded the framework, upload the .zip file to the root of your project and unzip it as follows:

```bash
$ cd my-project
$ unzip Simple-System-Info-master.zip -d simple-system-info
```

### Cloning the repository using git ###

*Dev release*
```bash
$ cd my-project
$ git clone git://github.com/ghost1227/Simple-System-Info/ simple-system-info
```

### Cloning the repository as a git submodule ###

*Dev release*
```bash
$ cd my-project
$ git submodule add git://github.com/ghost1227/Simple-System-Info/ simple-system-info
```

## Setting up SSI ##

Include SSI in your theme or plugin as follows:

```php
require_once('simple-system-info/simple-sysinfo.php');
$system_info = new Simple_System_Info();
$system_info->get();
```

## SSI Options ##

Currently, SSI only provides a single function - get(); However, this function takes several (optional) arguments:

```php
get( $show_inactive, $id, $class );
```

* $show_inactive - This is a boolean which determines whether or not to include inactive plugins in the plugin list. (Default: false)
* $id - This allows you to override the default ID assigned to the SSI textarea. (Default: system-info-box)
* $class - This allows you to assign a class (or classes) to the SSI textarea. None are assigned by default.

## FAQs ##

1. Why aren't there any FAQs?
 * Because you haven't asked any yet!

## Are you using SSI? ##

Send me an email at dgriffiths@ghost1227.com!

## Changelog ##

### Version 1.0.0 (August 19, 2013) ###

* Initial release
