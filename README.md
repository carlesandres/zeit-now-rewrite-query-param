# zeit-now-rewrite-query-param

When deployed to now v2 platform, this should create an API that when should respond on `/api/product/:id` with a JSON response like this:
```json
{
"productId": "the_id_provided"
}
```

This works as expected when running locally using `now dev` but one deployed to now v2, it actually responds with something like:

```json
{
"productId": ":productId?productId=the_id_provided"
}
```
