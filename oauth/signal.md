# Signal bot manager

## Change your phone number
This route allow you to change your phone number on the Amelia hub<br>
URL: `/pub/p1/signal/newPhone`<br>
Body: *POST*
```json
{
    "token": "API_KEY",
    "phone": "Your New Phone Number"
}
```
> Note that you will recice a code via message for phone validation

## Valid the phone number
This route allow you to check your phone number set before<br>
URL: `/pub/p1/signal/certifPhone`<br>
Body: *POST*
```json
{
    "token": "API_KEY",
    "code": "The code that your recive via Signal"
}
```

## Send message
You can now send message to your phone number via Signal ! <br>
URL: `/pub/p1/signal/send`<br>
Body: *POST*
```json
{
    "token": "API_KEY",
    "message": "your message"
}
```
