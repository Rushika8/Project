# ACME Metadata Visualization Tool (Looking Glass Schema Prototype)
### Project Overview
This project is a prototype visualization tool for exploring **metadata lineage and relationships** in the ACME dataset, inspired by the Looking Glass schema.  
Users can visualize tables, attributes, and dataflows in an interactive graph, helping analysts trace upstream and downstream data connections.
---
### Tech Stack
- **Frontend:** HTML, JavaScript, Cytoscape.js (for graph visualization)
- **Backend:** Node.js + Express  
- **Database:** PostgreSQL (accessed via pgAdmin)  
- **Version Control:** Git & GitHub
---
### How It Works
1. The backend (`server.js` and `api.js`) connects to the database and provides REST API endpoints.
2. The frontend (`index.html`, `main.js`, `graph.js`, etc.) visualizes metadata nodes and relationships using Cytoscape.js.
3. The sidebar and tooltips allow users to explore datasets, tables, and attributes interactively.
4. Future updates will support:
   - Lineage tracing (upstream/downstream flows)
   - Metadata filtering and search
   - Tabular and graph-based navigation
---
### Run Locally
To test the app on your computer:

```bash
# 1. Install dependencies
npm install

# 2. Start the server
npm run dev
# or
node server.js

# 3. Visit in your browser
http://localhost:3000
