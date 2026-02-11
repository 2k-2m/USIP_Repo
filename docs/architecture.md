\# Diseño de Arquitectura - SaaS Core



\## 1. Diagrama de Contexto (Mermaid)

```mermaid

graph LR

&nbsp; User((Usuario)) --> System\[SaaS Core]

&nbsp; System --> Stripe\[Gateway de Pagos]

&nbsp; System --> AWS\[S3 Storage]

