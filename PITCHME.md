## Salesforce <--> Banana Stand

#### John Fearnside
#### jfearnside@avvo.com

---
Banana Stand <==> Salesforce

---
## Banana Stand --> Salesforce
- Banana Stand --[HTTP]--> services
- Services --[Kafka]--> Stranger Forces
- Stranger Forces --[HTTP]--> Salesforce

---
## Salesforce --> Banana Stand
- Salesforce --[HTTP]--> Switchboard
- Switchboard --[HTTP]--> Services

---
## Banana Stand --> services
- via HTTP
- same as before

---
## Services --> Stranger Forces
- via Kafka
- Stranger Forces Elixir app
- Retries
- Denormalization via other services

---
## Kafka logging
- described in avvo_events gem
- produced using avvo_event_logger base gem
- AVDL (Apache Avro definition language)

---
## Stranger Forces --> Salesforce
- consumed using xxx
- HTTP
- Retries
- Credential caching

---
## Salesforce --> Switchboard
- HTTP (open)
- Proxies to services

---
## Resources
Slides: https://gitpitch.com/jwfearn/slides-sfbs


<!--
TODO: screenshots from BS and SF to show what data moves where

Intro - Chris
Batch - Gowthami
Realtime - John
Leveraging - Elisabeth
Execution - Chris

-->