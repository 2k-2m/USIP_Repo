### 2. `graphql-schema.md`
**El problema:** Tenías muchos caracteres extraños (`&nbsp;`) que rompen la validación de GraphQL. Aquí tienes el esquema limpio:

```graphql
# Esquema GraphQL - Pagos y Suscripciones

type Subscription {
  id: ID!
  planName: String!
  status: Status!
  nextBillingDate: String
}

enum Status { 
  ACTIVE 
  CANCELLED 
  PENDING 
}

type Query {
  getUserSubscriptions(userId: ID!): [Subscription]
}
