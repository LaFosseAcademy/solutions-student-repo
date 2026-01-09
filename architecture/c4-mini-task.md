# C4 Level 1 and 2 Task

Practice working with C4 level 1 and 2 diagarms

### Organisation

### Duration

You have **30 mins** to make as much progress on this task as possible.

Make sure to take breaks!

### Team

Solo task

## Brief

### Extend the C4 diagrams with Cloud Location‑History

You will add a cloud‑based storage component to both the Level 1 (Context) and Level 2 (Container) diagrams of the **Space‑Tracker** app. 
The new component will be called **Location‑History Service** and will allow the app to persist user location data and ISS‑pass predictions.

1. **Update the Level 1 Context diagram**
- Add a new **External System** shape.
- Rename it **Location‑History Service** and set the description to something like `Cloud store for user location & ISS‑pass history`.
- Create two new relations:
  - From the **Space‑Tracker App** to the **Location‑History Service** with the label “Writes location / pass data”.
  - From the **Location‑History Service** back to the **Space‑Tracker App** with the label “Provides stored location history”.
  - Position the new system to the right of the existing external systems for a clean layout.

4. **Update the Level 2 Container diagram**
- Inside the **Space‑Tracker App** system boundary, add a **Container** shape.
- Name it **Location‑History Adapter**, choose a technology (e.g., “Node.js / REST client”), and add a brief description such as “Writes/reads location and pass data to the cloud store”.
- Add the same **Location‑History Service** external system (if not already present from step 3) outside the boundary.
- Connect the new container with two relations:
  - From **Notification Scheduler** (or another relevant container) to **Location‑History Adapter** labeled “Saves upcoming pass predictions”.
  - From **Location‑History Adapter** to **Location‑History Service** labeled “Writes/reads location history”.
  - Optionally, connect **Mobile UI** to **Location‑History Adapter** if the UI will display past passes.
  
**You can complete the task using mermaid or draw.io**


