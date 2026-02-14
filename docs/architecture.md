# Diseño de Arquitectura - SaaS Core

## 1. Diagrama de Contexto (Mermaid)
```mermaid
graph LR
  User((Usuario)) --> System[SaaS Core]
  System --> Stripe[Gateway de Pagos]
  System --> AWS[S3 Storage]
```
## 2. Decisiones Tecnológicas

###Frontend: 
	React con Vite por su rapidez en desarrollo.
###Backend: 
	Node.js con arquitectura limpia (Clean Architecture).
###Infraestructura:
	Despliegue en contenedores para asegurar consistencia entre entornos de desarrollo y producción.
