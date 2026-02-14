
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
