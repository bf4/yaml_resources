## Rails database configuration

* Does not have a document header
* Is a mapping `:` of mappings.
* The default mapping is aliased as `&defaults`
* Other environments have the defaults mapping keys merged in `<<: *defaults`
* The default keys are over-written and customized for each environment.

```yaml
defaults: &defaults
  adapter: mysql2
  encoding: utf8
  reconnect: false
  pool: 5
  username: sqluser
  password: s3cret
  host: localhost

development:
  <<: *defaults
  database: app_development

test: &test
  <<: *defaults
  database: app_test

production:
  <<: *defaults
  username: productionsqluser
  password: productions3cret
  database: app_production
```
