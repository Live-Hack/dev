# Get user infos

This request allows to retrieve the public data of a user with his nickname.

## Use
Method: [!badge variant="primary" text="GET"]
```
https://www.live-hack.org/pub/v1/user/${username}
```

## Exemple
[Click to open](https://www.live-hack.org/pub/v1/user/alice)
```
https://www.live-hack.org/pub/v1/user/alice
```


## Response

==- [!badge variant="Success" text="Success"]
```json
{
    "username": "alice",
    "fullname": "Alice Snow",
    "points": 20,
    "grade": "admin",
    "bio": "Si la porte est fermée, pirate la fenêtre 💊",
    "avatar": "https://upload.live-hack.org/user/pp/alice.jpg",
    "website": "https://live-hack.org/"
}
```
==- [!badge variant="Danger" text="Error"]
If the response only contains the username, the user does not exist !
```json
{
    "username": "alice"
}
```
==-



