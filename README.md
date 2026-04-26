CS-340 Project Two: Grazioso Salvare Dashboard
Author: Breanna Bryant | Date: April 19, 2026

This JupyterDash application helps Grazioso Salvare explore animal shelter data and quickly identify dogs for water rescue, mountain or wilderness rescue, and disaster or tracking missions. It connects to MongoDB through a small CRUD Python module, displays an interactive Dash DataTable, recalculates a breed distribution chart from visible rows, and centers a map on the selected record. The included screenshot shows the header, mission filter, record count, and populated table in JupyterLab.

To reproduce the project, install Python 3.10 or 3.11 with JupyterLab. Install jupyter-dash, dash, dash-leaflet, plotly, pandas, pymongo, numpy, and matplotlib. Place ProjectTwoDashboard.ipynb, CRUD_Python_Module.py, and Grazioso Salvare Logo.png in one folder. Configure MongoDB credentials for a local instance or Atlas containing the AAC dataset, then run all notebook cells.

I write maintainable, readable, and adaptable programs by separating concerns, naming consistently, documenting intent, and keeping modules small. The CRUD module encapsulates database details and exposes simple methods the dashboard can reuse. Because the UI depends only on this interface, I can change credentials, hosts, or even the backing store with minimal edits. The same module could power other dashboards, CLI tools, or scheduled ETL jobs.

I approached the problem like a computer scientist by converting an open-ended request into testable requirements, building a minimal vertical slice, and iterating. Compared with earlier assignments, this project emphasized real-time interaction and fault tolerance. In the future I would add schema validation, environment-based configuration, and automated tests for callbacks and the CRUD layer.
