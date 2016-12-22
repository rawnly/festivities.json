# Festivities
A `json` file with all main international festivities.

Example:
```json
  "christmas" {
    "day": 25,
    "month": "December"
  }
```

Multiday festivities:
```json
"hanukkah": {
  "period": {
    "start": {
      "day": 24,
      "month": "December"
    },
    "end": {
      "day": 1,
      "month": "January"
    }
  }
}
```

## Usage
An example usage of this file can be

**Installation**
```bash
	npm install festivities --save
```

**Example**
```javascript
  const festivities = require('festivities');

  // This will return
  // { "day": 25, "month": "December" }
  console.log( festivities.christmas );

  // This will return 25
  console.log( festivities.christmas.day );

  // This will return `December`
  console.log( festivities.christmas.month );

  // For multiday festivities
  // in 2016 this will return 24
  console.log( festivities.hanukkah.start.day );

  // and that 1
  console.log( festivities.hanukkah.end.day );

  // Print full date

  // abbreviation
  var hanukkah = festivities.hanukkah;

  // this will return "24 December"
  console.log( `${hanukkah.start.day}/${hanukkah.start.month}`);

```

## Hack
You can also add other **festivities** doing the following steps:

1. Fork this repo: https://github.com/rawnly/festivities.json/fork
2. Create your festivity branch (git checkout -b my-new-festivity)
3. Commit your changes (git commit -am 'Added a new festivity')
4. Push to the branch (git push origin my-new-festivity)
5. Create a new Pull Request

### Please follow the file structure.

## Supported Festivities:

- christmas
- epifany
- new_year
- chinese_new_year
- hanukkah
- halloween
- valentines
- starwars_day
- earth_day


# TODO
- [x] Add multiday festivities as requested in [#1](https://github.com/Rawnly/festivities.json/issues/1)
- [ ] Write an pull guide.
