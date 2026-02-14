### 2. Archivo: `graphql-schema.md`

```graphql
# Esquema GraphQL - Pagos y Suscripciones

"""
Representa una suscripción activa de un cliente en el sistema SaaS.
"""
type Subscription {
  id: ID!
  planName: String!
  status: Status!
  nextBillingDate: String
}

"""
Estados posibles de una suscripción.
"""
enum Status { 
  ACTIVE 
  CANCELLED 
  PENDING 
}

type Query {
  """
  Obtiene el historial y estado actual de suscripciones de un usuario.
  """
  getUserSubscriptions(userId: ID!): [Subscription]
}
