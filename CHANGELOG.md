# Changelog

All notable changes to `ray` will be documented in this file

## 1.8.0 - 2021-01-14

- add a check for YiiRay's instance

## 1.7.2 - 2021-01-13

- when passing `null`, let argument convertor return `null`

## 1.7.1 - 2021-01-13

- improve return type of ray function

## 1.7.0 - 2021-01-13

- support multiple arguments to `toJson()` and `json()` (#148)

## 1.6.1 - 2021-01-13

- prevent possible memory leak (#143)

## 1.6.0 - 2021-01-13

- add `file` function (#134)

## 1.5.10 - 2021-01-13

- allow better compatibility with WordPress

## 1.5.9 - 2021-01-13

- ignore package version errors

## 1.5.8 - 2021-01-13

- ignore package check errors

## 1.5.7 - 2021-01-13

- remove unneeded symfony/console dependency

## 1.5.6 - 2021-01-13

- allow lower dependencies

## 1.5.5 - 2021-01-11

- split origin factory in overridable functions

## 1.5.4 - 2021-01-11

- support WordPressRay

## 1.5.3 - 2021-01-10

- fix for traces of WordPress

## 1.5.2 - 2021-01-10

- colorize app frames

## 1.5.1 - 2021-01-10

- polish json functions

## 1.5.0 - 2021-01-09

- add `json` function

## 1.4.0 - 2021-01-09

- add `rd` function

## 1.3.7 - 2021-01-09

- add `vendor_frame` attribute to frames

## 1.3.6 - 2021-01-09

- allow older version of uuid package

## 1.3.5 - 2021-01-09

- fix search for `$indexOfRay` to include calls from the parent directory (#80)

## 1.3.4 - 2021-01-08

- prevent warning if `open_basedir` is enabled

## 1.3.3 - 2021-01-08

- do not require Composer 2

## 1.3.2 - 2021-01-08

- prevent ray from blowing up when there is no config file

## 1.3.1 - 2021-01-08

- do not blow up when the Ray app is not running

## 1.3.0 - 2021-01-08

- add support for `remote_path` and `local_path` config values

## 1.2.0 - 2021-01-08

- add `pass` function

## 1.1.3 - 2021-01-08

- prevent exception when installing in an Orchestra powered testsuite

## 1.1.2 - 2021-01-08

- enforce Composer 2 requirement

### 1.1.1 - 2021-01-08

- fix for repeated calls to `ray()` throwing an exception (#30)

## 1.1.0 - 2021-01-07

- add `makePathOsSafe`
- fix tests

## 1.0.1 - 2021-01-07

- fix default settings

## 1.0.0 - 2021-01-07

- initial release
