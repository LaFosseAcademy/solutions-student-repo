# Software Architecture task

Practice selecting an appropriate architecture for a problem

### Duration

You have **1 hour** to make as much progress on this task as possible.

Make sure to take breaks!

### Team

Group task

## Brief: To-Do App
A company wants to build a real‑time collaborative “To‑Do” web app that will be used by small teams (2‑10 members).
The product road-map includes:
1. Core features – user sign‑up/login, CRUD on to‑do items, shared lists with live updates.
2. Future extensions – optional integrations with external calendars, a mobile client, and a reporting dashboard.
3. Non‑functional constraints:
   - Launch deadline: 3 months (minimum viable product).
   - Scalability: must handle up to 5k concurrent users at launch, with the ability to grow to 100k later.
   - Team size: 4 developers now, expanding to 8 in six months.
   - Operational budget: limited – prefer fewer moving parts for the MVP.
   
## Deliverables
1. A table that lists the five patterns you will consider (MVC, Layered, Monolith, Event‑Driven, Microservices). For each pattern, fill in the following columns: 
   - Fit for MVP deadline
   - Ease of scaling later
   - Team-size suitability
   - Operational complexity
   - Support for future extensions
2. Identify the two-to-three patterns that score highest overall and explain why they stand out for this scenario.
3. Choose one architecture as the best fit for the MVP and justify the decision in terms of the constraints above. Mention any “phased approach” you would adopt (e.g., start with a monolith and later extract services).
4. **BONUS:** A quick C4-style container diagram of the chosen architecture.
