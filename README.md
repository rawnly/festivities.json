# Festivities

A `json` file with all main international festivities.

Example:
```json
  "christmas" {
    "day": 25,
    "month": "December"
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
  const festivities = require('../path/to/festivities');

  // This will return
  // { "day": 25, "month": "December" }
  console.log( festivities.christmas );

  // This will return 25
  console.log( festivities.christmas.day );

  // This will return `December`
  console.log( festivities.christmas.month );
```

## Hack
You can also add other **festivities** doing the following steps:

1. Fork this repo: https://github.com/rawnly/festivities.json/fork
2. Create your festivity branch (git checkout -b my-new-festivity)
3. Commit your changes (git commit -am 'Added a new festivity')
4. Push to the branch (git push origin my-new-festivity)
5. Create a new Pull Request
