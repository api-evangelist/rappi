# Rappi (rappi)

Rappi is a Colombian-founded pan-Latin American super-app headquartered in Bogotá, with regional hubs in São Paulo and Mexico City. Founded in 2015 by Simón Borrero, Sebastián Mejía, and Felipe Villamarín, and accelerated through Y Combinator's W16 batch, Rappi operates across Argentina, Brazil, Chile, Colombia, Costa Rica, Ecuador, Mexico, Peru, and Uruguay. The platform bundles on-demand delivery (restaurants, groceries via "Súper" and Turbo Fresh, pharmacies, retail, alcohol) with consumer fintech (RappiPay, RappiCard, RappiCash) and adjacent services such as RappiTravel and the RappiPrime subscription. Rappi's developer surface is operated through its Partners program at dev-portal.rappi.com, where approved restaurants, retailers, and middleware providers obtain OAuth 2.0 client credentials to integrate with a REST API for menu and catalog management, store availability, order lifecycle events, financial reconciliation, and webhook subscriptions. Access is not self-serve — a Rappi business contact must approve onboarding, after which partners receive development-environment credentials and an integration path to production. SoftBank-backed since 2019, Rappi competes regionally with iFood, Uber Eats, and DiDi Food, with fintech ambitions overlapping Nubank, Mercado Pago, and regional neobanks.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/rappi/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Delivery, Food Delivery, Grocery Delivery, On-Demand, Last Mile, Logistics, Super App, Fintech, Payments, Marketplace, Latin America, Colombia

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Rappi Partners REST API

The Rappi Partners REST API is the integration surface used by approved restaurants, grocery and retail merchants, and middleware/POS providers to operate on the Rappi marketplace. Authentication is OAuth 2.0 client-credentials — partners receive a client_id and client_secret from Rappi after manual onboarding, exchange them at POST token/login/integrations for a bearer access token, and re-issue the token at least weekly. The API exposes endpoints for menu and catalog management, product and store availability toggling, retrieving store data, accepting and progressing user orders, and a separate Financial surface for reconciliation. A parallel "Rests API" track covers the same operations for the restaurant vertical. Webhook events deliver order lifecycle and store updates to partner-hosted callback URLs. Rappi enforces a 45-second minimum gap between requests and expects integrators to maintain a 98% API success rate; production access is gated on certification by the Rappi integrations team.

**Human URL:** [https://dev-portal.rappi.com/](https://dev-portal.rappi.com/)

#### Tags:

 - Orders, Menus, Catalog, Availability, Stores, Webhooks, Financial, OAuth, REST

#### Properties

- [Documentation](https://dev-portal.rappi.com/)
- [APIReference](https://dev-portal.rappi.com/en/api-reference/)
- [GettingStarted](https://dev-portal.rappi.com/en/api-reference/)
- [Authentication](https://dev-portal.rappi.com/en/api-reference/authentication/)
- [Webhooks](https://dev-portal.rappi.com/en/api-reference/webhooks/)

## Common Properties

- [Website](https://www.rappi.com/)
- [About](https://about.rappi.com/about-us)
- [DeveloperPortal](https://dev-portal.rappi.com/)
- [APIReference](https://dev-portal.rappi.com/en/api-reference/)
- [Authentication](https://dev-portal.rappi.com/en/api-reference/authentication/)
- [Webhooks](https://dev-portal.rappi.com/en/api-reference/webhooks/)
- [IntegrationStandards](https://dev-portal.rappi.com/integration-standards/)
- [FAQ](https://dev-portal.rappi.com/en/faqs/)
- [Deprecations](https://dev-portal.rappi.com/en/deprecations/)
- [Merchants](https://merchants.rappi.com/)
- [StoreSignUp](https://mitienda.rappi.com.mx/)
- [Couriers](https://soyrappi.com.mx/)
- [RappiPay](https://www.rappipay.mx/)
- [Blog](https://blog.rappi.com/)
- [GitHubOrganization](https://github.com/rappiinc)
- [LinkedIn](https://www.linkedin.com/company/rappi)
- [YCombinator](https://www.ycombinator.com/companies/rappi)

## Features

| Name | Description |
|------|-------------|
| On-Demand Delivery | Restaurant, grocery (Súper), pharmacy, retail, and alcohol delivery fulfilled by the Rappi courier fleet across nine LatAm countries. |
| Turbo Fresh | Sub-15-minute grocery and convenience delivery from Rappi-operated dark stores in major metropolitan areas. |
| RappiPay & RappiCard | Consumer fintech wallet, debit, and co-branded credit card products embedded in the super-app and operated as regulated entities in select markets. |
| RappiTravel | In-app flights, hotels, and travel booking surface integrated with the Rappi wallet and loyalty stack. |
| RappiPrime Subscription | Recurring membership offering free delivery, exclusive discounts, and partner perks across the super-app verticals. |
| Partners Developer Portal | OAuth-secured REST API for menus, availability, orders, stores, financial reconciliation, and webhooks, gated behind manual partner onboarding. |

## Use Cases

| Name | Description |
|------|-------------|
| POS & Aggregator Integration | Restaurant POS vendors and order aggregators sync menus and push/pull orders between merchant systems and Rappi storefronts. |
| Grocery & Retail Catalog Sync | Supermarket and convenience chains keep large SKU catalogs and real-time stock availability synchronized with Rappi store pages. |
| Order Lifecycle Automation | Brands receive Rappi orders via webhook, route them to kitchen or fulfillment systems, and progress status back through the API. |
| Financial Reconciliation | Merchants pull payout, commission, and settlement data through the Financial endpoints for accounting and FP&A pipelines. |
| Last-Mile as a Service | Enterprise brands tap the Rappi courier fleet for branded last-mile delivery in LatAm metros. |

## Integrations

| Name | Description |
|------|-------------|
| Restaurant POS Systems | Middleware providers connect kitchen and POS platforms to the Rappi Rests API for menu and order flow. |
| Grocery & Retail ERPs | Catalog, pricing, and inventory systems push availability updates through the Partners API. |
| Payment Networks | RappiPay and RappiCard integrate with regional card networks and local payment rails per country. |
| Travel Suppliers | RappiTravel aggregates flight and hotel inventory from third-party GDS and travel partners. |

## Solutions

| Name | Description |
|------|-------------|
| Restaurants | Onboarding, menu management, order capture, and reconciliation tools for restaurant brands on the Rappi marketplace. |
| Grocery & Retail | Catalog, stock, and store-availability tooling for supermarket, convenience, and specialty retail partners. |
| Brands & Enterprises | Last-mile fulfillment and Rappi-native commerce for enterprise brands seeking LatAm coverage. |
| Consumers | The Rappi super-app for delivery, fintech, travel, and Prime subscription benefits across nine countries. |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
