# Jupyter-PHP Installer ([Main Page](https://litipk.github.io/Jupyter-PHP-Installer/))

[![Author](http://img.shields.io/badge/author-@castarco-blue.svg?style=flat-square)](https://twitter.com/castarco)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)
[![Packagist Version](https://img.shields.io/packagist/v/Litipk/jupyter-php.svg?style=flat-square)](https://packagist.org/packages/Litipk/jupyter-php)

## Introduction

[**Jupyter-PHP**](https://github.com/Litipk/Jupyter-PHP) is a PHP kernel for [*Jupyter*](http://jupyter.org). This
repository holds an installer to make easier installing the Jupyter-PHP kernel.

## Getting started

Go to the [main page](https://litipk.github.io/Jupyter-PHP-Installer/) and follow the instructions.

## Learn more

 * [Chat Room](https://gitter.im/Litipk/Jupyter-PHP) : If you want to have a real-time chat with other Jupyter-PHP users or developers, you can do it here.
 * [Group / Mail List](https://groups.io/g/jupyter-php) : If a chat room isn't enough to post your doubts or ideas, you can join to our mail list.

## How to contribute

 * First of all, you can take a look on the [bugtracker](https://github.com/Litipk/Jupyter-PHP-Installer/issues) and decide if there is something that you want to do :wink: . If you think there are missing improvements in this file, then you are invited to modify the TODO list.
 * You can also send us bug reports using the same bugtracker.
 * If you are really interested on helping to improve Litipk\BigNumbers, we recommend to read the [contributing guidelines](https://github.com/Litipk/Jupyter-PHP-Installer/blob/master/CONTRIBUTING.md).
 
## Addendum

If you just want to run the installer from this repository without building a phar file you can do the following:

```bash
composer install
composer execute install
```

To create an installer that works with the latest composer, you can run. Unfortunately this will need to be modified to work for Windows.

```bash
chmod +x bin/build.sh && bin/build.sh
```

The other important thing is to make sure you have the ZeroMQ extension installed or you will hit problems. The Jupyter notebook needs it for communicating with the language engine.

[Installing ZeroMQ](https://gist.github.com/qutek/42889d82a4cbebf0e801943a9addbbab)

And finally after you have your successful install

```bash
jupyter notebook
```

![](images/9f8869ef.png)

## License

Jupyter-PHP and its installer are licensed under the [MIT License](https://github.com/Litipk/Jupyter-PHP-Installer/blob/master/LICENSE).
