# YAML recipes

## Rails database configuration

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
