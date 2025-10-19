# alx-project-7

A small project demonstrating use of GraphQL queries and how to call a GraphQL endpoint.

## Quick start
- Run your GraphQL server (for example at http://localhost:4000/graphql).
- Use GraphiQL/Playground or curl to execute queries.

## Example GraphQL query
Use this query to fetch a user by id:

```graphql
query GetUser {
  user(id: "1") {
    id
    name
    email
  }
}
```

## Example using curl
Execute the same query via curl:

```bash
curl -X POST http://localhost:4000/graphql \
  -H "Content-Type: application/json" \
  --data '{"query":"query GetUser { user(id: \"1\") { id name email } }"}'
```

## Notes
- Replace the endpoint and field names to match your schema.
- For authenticated endpoints add an Authorization header:
  -H "Authorization: Bearer <TOKEN>"


