## Speaker roster at a conference

Taken from [GoGaRuCo 2013 site](https://github.com/gogaruco/gogaruco.github.com/blob/2013/data/speakers.yml)

* Begins with a document header that does not specify a yaml version. e.g. `--- %YAML%1.1`
* Is a mapping `:` of mappings.
  * The items in the roster mapping are mappings.
  * The items in the feature and sorted mappings are sequences `-`.
* The key for each speaker mapping on the roster is aliased as that key name `&atwood`
* The speakers on the roster are referenced in subsequent mappings such as featured with an anchor `*gray`
* The folded block followed by indentation `>` in the bios key concatenates the indented lines into one for convenient formatting


```yaml
---
roster:
  atwood: &atwood
    slug: atwood
    name: Jeff Atwood
    twitter: codinghorror
    bio: >
      You may know Jeff Atwood from his <a href="http://codinghorror.com/">Coding Horror</a> blog or his
      work on <a href="http://stackoverflow.com/">stackoverflow.com</a>. Now he is learning Ruby and using
      it to build a new generation of forum software called <a href="http://discourse.org">Discourse</a>.
      He lives in Berkeley, CA with his wife, two cats, three children, and lots of computers. His power
      animal is the wumpus.
  gray: &gray
    slug: gray
    name: James Edward Gray II
    twitter: JEG2
    bio: >
      Constructed in the future to speak to the machines and sent back in time to prepare the humans for
      what comes next, James Edward Gray II might literally be built to be a programmer. Sure, there are
      more advanced models, but James has fought in the developer trenches and the battles have changed
      him. He now spends most of his time trying to download what he has learned into the brains of others
      by writing books, speaking at conferences, and contributing to the Ruby Rogues podcast.
  harms: &harms
    slug: harms
    name: Angela Harms
    twitter: angelaharms
    bio: >
      Angela Harms is an agile developer, coach, facilitator, and instigator. She loves beautiful code
      that emerges from collaboration, and learning new ways to make it work. She lives in a community of
      nerds called MakerHouse in Cleveland’s historic Ohio City, and you can learn more about her work at
      <a href="http://maitria.com/">maitria.com</a>.
featured:
  - *gray
  - *harms
sorted:
  - *atwood
  - *gray
  - *harms
```

```json
{
  "roster": {
    "atwood": {
      "slug": "atwood",
      "name": "Jeff Atwood",
      "twitter": "codinghorror",
      "bio": "You may know Jeff Atwood from his <a href=\"http:\/\/codinghorror.com\/\">Coding Horror<\/a> blog or his work on <a href=\"http:\/\/stackoverflow.com\/\">stackoverflow.com<\/a>. Now he is learning Ruby and using it to build a new generation of forum software called <a href=\"http:\/\/discourse.org\">Discourse<\/a>. He lives in Berkeley, CA with his wife, two cats, three children, and lots of computers. His power animal is the wumpus.\n"
    },
    "gray": {
      "slug": "gray",
      "name": "James Edward Gray II",
      "twitter": "JEG2",
      "bio": "Constructed in the future to speak to the machines and sent back in time to prepare the humans for what comes next, James Edward Gray II might literally be built to be a programmer. Sure, there are more advanced models, but James has fought in the developer trenches and the battles have changed him. He now spends most of his time trying to download what he has learned into the brains of others by writing books, speaking at conferences, and contributing to the Ruby Rogues podcast.\n"
    },
    "harms": {
      "slug": "harms",
      "name": "Angela Harms",
      "twitter": "angelaharms",
      "bio": "Angela Harms is an agile developer, coach, facilitator, and instigator. She loves beautiful code that emerges from collaboration, and learning new ways to make it work. She lives in a community of nerds called MakerHouse in Cleveland\u2019s historic Ohio City, and you can learn more about her work at <a href=\"http:\/\/maitria.com\/\">maitria.com<\/a>.\n"
    }
  },
  "featured": [
    {
      "slug": "gray",
      "name": "James Edward Gray II",
      "twitter": "JEG2",
      "bio": "Constructed in the future to speak to the machines and sent back in time to prepare the humans for what comes next, James Edward Gray II might literally be built to be a programmer. Sure, there are more advanced models, but James has fought in the developer trenches and the battles have changed him. He now spends most of his time trying to download what he has learned into the brains of others by writing books, speaking at conferences, and contributing to the Ruby Rogues podcast.\n"
    },
    {
      "slug": "harms",
      "name": "Angela Harms",
      "twitter": "angelaharms",
      "bio": "Angela Harms is an agile developer, coach, facilitator, and instigator. She loves beautiful code that emerges from collaboration, and learning new ways to make it work. She lives in a community of nerds called MakerHouse in Cleveland\u2019s historic Ohio City, and you can learn more about her work at <a href=\"http:\/\/maitria.com\/\">maitria.com<\/a>.\n"
    }
  ],
  "sorted": [
    {
      "slug": "atwood",
      "name": "Jeff Atwood",
      "twitter": "codinghorror",
      "bio": "You may know Jeff Atwood from his <a href=\"http:\/\/codinghorror.com\/\">Coding Horror<\/a> blog or his work on <a href=\"http:\/\/stackoverflow.com\/\">stackoverflow.com<\/a>. Now he is learning Ruby and using it to build a new generation of forum software called <a href=\"http:\/\/discourse.org\">Discourse<\/a>. He lives in Berkeley, CA with his wife, two cats, three children, and lots of computers. His power animal is the wumpus.\n"
    },
    {
      "slug": "gray",
      "name": "James Edward Gray II",
      "twitter": "JEG2",
      "bio": "Constructed in the future to speak to the machines and sent back in time to prepare the humans for what comes next, James Edward Gray II might literally be built to be a programmer. Sure, there are more advanced models, but James has fought in the developer trenches and the battles have changed him. He now spends most of his time trying to download what he has learned into the brains of others by writing books, speaking at conferences, and contributing to the Ruby Rogues podcast.\n"
    },
    {
      "slug": "harms",
      "name": "Angela Harms",
      "twitter": "angelaharms",
      "bio": "Angela Harms is an agile developer, coach, facilitator, and instigator. She loves beautiful code that emerges from collaboration, and learning new ways to make it work. She lives in a community of nerds called MakerHouse in Cleveland\u2019s historic Ohio City, and you can learn more about her work at <a href=\"http:\/\/maitria.com\/\">maitria.com<\/a>.\n"
    }
  ]
}
```
