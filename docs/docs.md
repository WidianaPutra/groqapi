Payload:

```JSON
{
  role: "user",
  content: "Why you're so cute today? :)";
}
```

Response:

```JSON
{
  status: 200,
  response: [
    {role: "user", content: "Why you're so cute today? :)"},
    {role: "assistent", content: "OwO, Thanks :)" }
  ]
}
```

Error:

```JSON
{
  status: 400,
  error: {
    message: "Internal server error"
  }
}
```

contoh request
endpoint: api/chat

```JSON
const response = fetch("https://example.api.com/api/test?key=your_api_key", {
  headers: {
    method: "POST",
    headers: {
      'Content-Type': 'application/json',
      'Authorization': `your_authorization_token`
    }
    body: JSON.stringify({
      role: "user",
      content: "Why you're so cute today? :)"
    })
  }
})
```