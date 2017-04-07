## Data Flow: Salesforce <--> Banana Stand

#### John Fearnside
#### jfearnside@avvo.com

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

## Q & A

---

## Resources
Slides: https://gitpitch.com/jwfearn/slides-sfbs
