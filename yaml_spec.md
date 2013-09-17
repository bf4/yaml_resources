- YAML: A human-friendly data serialization standard
  1. human-friendly
  2. data serialization
  3. standard
- Spec overview with vocabulary
  - vs. JSON, XML, internal DSL
- Spec Implementation details (libraries)
  = 1.0, 1.1, 1.2


## YAML Spec and Terminology

* [YAML Ain’t Markup Language (YAML™) Version 1.2](http://yaml.org/spec/1.2/spec.html)

```yaml
%YAML 1.2
---
YAML: YAML Ain't Markup Language

What It Is: YAML is a human friendly data serialization
  standard for all programming languages.
```

* Symbols
* Classes
* [JSON superset](http://yaml.org/spec/1.2/spec.html#id2759572)
  * The primary objective of this revision is to bring YAML into compliance with JSON as an official subset. YAML 1.2 is compatible with 1.1 for most practical applications - this is a minor revision. An expected source of incompatibility with prior versions of YAML, especially the syck implementation, is the change in implicit typing rules. We have removed unique implicit typing rules and have updated these rules to align them with JSON's productions. In this version of YAML, boolean values may be serialized as “true” or “false”; the empty scalar as “null”. Unquoted numeric values are a superset of JSON's numeric production. Other changes in the specification were the removal of the Unicode line breaks and production bug fixes. We also define 3 built-in implicit typing rule sets: untyped, strict JSON, and a more flexible YAML rule set that extends JSON typing.

###  Vocabulary

