
# Magic Lambda Config

[![Build status](https://travis-ci.org/polterguy/magic.lambda.config.svg?master)](https://travis-ci.org/polterguy/magic.lambda.config)

This project provides configuration settings slots for [Magic](https://github.com/polterguy/magic). The project provides one
single slot, allowing you to retrieve configuration settings from your configuration file as follows.

* __[config]__ - Returns the configuration value from your configuration file with the specified key.

You can supply a _"path"_ such as _"foo:bar"_, which will traverse into your _"foo"_ config setting, find its _"bar"_ key,
and return the value of your _"bar"_ key. Below is an example of usage.

```
config:"foo:bar"
```

Assuming your configuration file looks like the following.

```json
{
   "foo": {
      "bar": 42
   }
}
```

... afterwards the value of your __[config]__ node will be the following.

```
foo:int:42
```

## License

Although most of Magic's source code is Open Source, you will need a license key to use it.
[You can obtain a license key here](https://servergardens.com/buy/).
Notice, 7 days after you put Magic into production, it will stop working, unless you have a valid
license for it.

* [Get licensed](https://servergardens.com/buy/)
