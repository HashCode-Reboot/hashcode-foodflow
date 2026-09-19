# Architecture — FoodFlow

```mermaid
flowchart TB
 P[Producteurs] --> APP[Application]
 APP --> API[FoodFlow API]
 API --> INV[Inventaire]
 API --> STO[Stockage]
 API --> LOG[Logistique]
 API --> MKT[Offre / demande]
 API --> AL[Alertes]
 MKT --> OPT[Optimisation]
 STO --> IMP[Mesure des pertes]
 LOG --> IMP
```

## Principes

Mobile-first, synchronisation tolérante aux coupures, données horodatées, traçabilité de provenance et séparation entre observations et prédictions.

Les recommandations de prix, demande ou logistique doivent être présentées comme des estimations et évaluées contre les résultats terrain.