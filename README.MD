# Tickety Locale

This is the official github repo for the Tickety locale files. Meant to make it easier for people to add their own languages into the mix.

Feel free to open a PR and add your own language. Everyone that adds a language/makes a big contribution gets a premium token 😀.

### So, how would I add a language?

First off, PRs should be made to the `develop` branch, we don't merge PRs directly into the `master` branch.

Here is an example of what the file looks like: 
```json
{ 
  "en": { // This is the beginning of a new language, this should be your language code
    "generic": {
      "updated": "The :field: has updated!"
    },
    "cmds": {
      "help": {
        "description": "Show all of my commands"
      }
    }
  },
  
  "nl": {
    "generic": {
      "updated": "De :field: is geupdate!" // As you can see the "updated" and the ":field:" should NOT be translated.
    },
    "cmds": {
      "help": {
        "description": "Laat al mijn commando's zien"
      }
    }
  }
}
```
The fields within colons should NOT be translated, those are variables that are hooked into from the code.
Nor should the keys be translated, only the values of the JSON object.