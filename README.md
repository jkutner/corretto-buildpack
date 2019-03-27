# Amazon Corretto JDK Buildpack

This [buildpack](https://devcenter.heroku.com/articles/buildpacks) will install the [Amazon Corretto](https://docs.aws.amazon.com/corretto/index.html) runtimes.

## Usage

This buildpack can be used with the [Heroku Java buildpack](https://github.com/heroku/heroku-buildpack-java/blob/master/bin/compile) to replace the default JDK by running:

```
$ heroku buildpacks:set jdk/corretto
$ heroku buildpacks:add heroku/java
```

## Customizing

You can customize the version of Corretto by setting the following config vars:

* `CORRETTO_URL`
* `CORRETTO_CHECKSUM`

For more information on acceptable values, see the [Corretto downloads page](https://docs.aws.amazon.com/corretto/latest/corretto-8-ug/downloads-list.html).

## License

MIT
