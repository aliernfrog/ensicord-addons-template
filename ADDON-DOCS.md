# Ensicord add-ons
Ensicord add-ons are simple JSON objects which are parsed into [Addon class](https://github.com/aliernfrog/ensicord/blob/compose/app/src/main/java/com/aliernfrog/ensicord/data/Addon.kt) in Ensicord

## Add-on object example
```kotlin
{
  "name": String,
  "description": String,
  "thumbnailUrl": String?,
  "setAppTheme": String?,
  "setEnsiUserName": String?,
  "setEnsiWords": Array<String>?,
  "addEnsiWords": Array<String>?,
  "setEnsiVerbs": Array<String>?,
  "addEnsiVerbs": Array<String>?
}
```

### Description
- `name`: Required, name of the add-on
- `description`: Required, description of the add-on
- `thumbnailUrl`: Optional, URL of image which will be displayed before add-on name
- `setAppTheme`: Optional, sets dark mode preference of Ensicord. `SYSTEM` (default), `DARK` and `LIGHT` are available
- `setEnsiUserName`: Optional, sets user name of Ensi in Ensicord
- `setEnsiWords`: Optional, overwrites current saved words set
- `addEnsiWords`: Optional, adds to the saved words set if it doesn't have the element already
- `setEnsiVerbs`: Optional, overwrites current saved verbs set
- `addEnsiVerbs`: Optional, adds to the saved verbs set if it doesn't have the element already