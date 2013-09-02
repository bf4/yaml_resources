## Rails database configuration

* Does not have a document header
* Is a mapping `:` of mappings.
* The default mapping is aliased as `&defaults`
* Other environments have the defaults mapping keys merged in `<<: *defaults`
* The default keys are over-written and customized for each environment.


<table>
<thead>
  <tr>
  <th>YAML</th>
  <th>JSON</th>
  </tr>
</thead>
<tbody>
<tr><td>

<pre>

    defaults: &defaults
      adapter: mysql2
      encoding: utf8
      reconnect: false
      pool: 5
      username: sqluser
      password: s3cret
      host: localhost
    
    development:
      &lt;&lt;: *defaults
      database: app_development
    
    test: &test
      &lt;&lt;: *defaults
      database: app_test
    
    production:
      &lt;&lt;: *defaults
      username: productionsqluser
      password: productions3cret
      database: app_production

</pre>

</td><td>

<pre>

    {
      "defaults": {
        "adapter": "mysql2",
        "encoding": "utf8",
        "reconnect": false,
        "pool": 5,
        "username": "sqluser",
        "password": "s3cret",
        "host": "localhost"
      },
      "development": {
        "adapter": "mysql2",
        "encoding": "utf8",
        "reconnect": false,
        "pool": 5,
        "username": "sqluser",
        "password": "s3cret",
        "host": "localhost",
        "database": "app_development"
      },
      "test": {
        "adapter": "mysql2",
        "encoding": "utf8",
        "reconnect": false,
        "pool": 5,
        "username": "sqluser",
        "password": "s3cret",
        "host": "localhost",
        "database": "app_test"
      },
      "production": {
        "adapter": "mysql2",
        "encoding": "utf8",
        "reconnect": false,
        "pool": 5,
        "username": "productionsqluser",
        "password": "productions3cret",
        "host": "localhost",
        "database": "app_production"
      }
    }

</pre>

</td></tr>
</tbody></table>
