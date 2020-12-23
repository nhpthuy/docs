---
title: "Database Settings" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/database-settings.html 
redirect_from:
    - "/display/KD/Database+Settings/"
    - "/display/KD/Database%20Settings/"
    - "/x/tgFO/"
    - "/katalon-studio/docs/database-settings/"
description: 
---
Outline:
- Why this doc?

Due to the Open-source library compliance issue, we decided to remove mySQL from our built-in libraries list. This will impact the configuration of all existing projects having configured MySQL DB connection
- Preconditions

Prior to 7.9: mySQL is one of the built-in libraries, which allows the built-in database connection support.

From 7.9 onwards: 

Remove MySQL from Katalon Studio built-in function

- Limitations

- Requirements

- How-to guide?

To use MySQL DB:
1. Download the DB jar file: https://dev.mysql.com/downloads/connector/j/
2. Add the downloaded jar file to the external library of a project: Project/settings/library management/ browse to the jar file
3. Config Database connection: Project/settings/database/specify username, password, connection URL click test connection
