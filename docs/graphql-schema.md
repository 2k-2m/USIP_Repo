\# Esquema GraphQL - Pagos y Suscripciones



```graphql

type Subscription {

&nbsp; id: ID!

&nbsp; planName: String!

&nbsp; status: Status!

&nbsp; nextBillingDate: String

}



enum Status { ACTIVE, CANCELLED, PENDING }



type Query {

&nbsp; getUserSubscriptions(userId: ID!): \[Subscription]

}

