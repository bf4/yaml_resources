
- Use-cases aka why bother with YAML?
  - Marshaling (serialize) objects
    - arbitrary objects
    - Ruby > 1.9.2 / Psych >= 1.0.0 allows arbitrary !ruby/hash classes -> #initialize then #[]= (normally #allocation, instance_variable_set) -> symbol DoS
  - configuration
    - at top of markdown file: jekyll, metadown
  - data store (e.g. pstore)
- Recipes
  - i18n
