<h1 align="center">Conequate_Core</h1> 

<div align="center">
  <p>Simplifies calling Magento data structures.</p>
  <img src="https://img.shields.io/badge/magento-2.2%20|%202.3-brightgreen.svg?logo=magento&longCache=true&style=flat-square" alt="Supported Magento Versions" />
  <a href="https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity" target="_blank"><img src="https://img.shields.io/badge/maintained%3F-yes-brightgreen.svg?style=flat-square" alt="Maintained - Yes" /></a>
  <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
</div>

## Table of contents

- [Summary](#summary)
- [Installation](#installation)
- [License](#license)

## Summary

A base module that is used for all the extensions contained a `menu.xml` base, in order to use we need to add `parent="Conequate_Core"` in our menu item.

```xml
        <add id="Sample_Module::conequate"
             title="Conequate"
             module="Sample_Module"
             sortOrder="50"
             parent="Conequate_Core"
             resource="Sample_Module::menu" />
```


## Installation

```sh
composer require conequate/core
bin/magento module:enable Conequate_Core
bin/magento setup:upgrade
```

## License

[MIT](https://opensource.org/licenses/MIT)