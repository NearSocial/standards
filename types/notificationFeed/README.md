# Notification Feed [Draft]

## Schema

The SCHEMA is to be described.

Users get different type of notifications from users. 
It should be used when you need a user to be notified of some event. This event might even happen outside Near Social. For example
- You've been mentioned on a widget.
- You are requested to do something on a website you've given permission to send you notifications

On this notifications, you might even want to have a link to be redirected to the corresponding place, always considering security.

## Example 1

In this case, Alice would create a notification to Bob letting Bob know Alice mentioned Bob in Alice's main page with no message

```json
{
  "alice.near": {
    "index": {
      "notify": {
        "key": "bob.near",
        "value": {
          "type": "mention",
          "item": {
            "type": "social",
            "path": "alice.near/post/main",
            "blockHeight": 88260018,
            "message": ""
          }
        }
      }
    }
  }
}
```

## Example 2

In this case, Alice would create a notification alert to Bob letting Bob know Alice played in a game along with a link to the website. For this, it is ideal to have either a whitelisted and blacklisted websites and an alert for not yet listed pages telling the user they are getting out of Near Social so they can proceed under their own risk.

```json
{
  "alice.near": {
    "index": {
      "notify": {
        "key": "bob.near",
        "value": {
          "type": "alert",
          "item": {
            "type": "social",
            "path": "https://near.gaming",
            "blockHeight": 88260018,
            "message": "It's your turn"
          }
        }
      }
    }
  }
}
```