# GoBacolod: MCP-Governed AI-Assisted Jeepney Routing and Safe Navigation System

## Problem Statement

In Bacolod City, jeepneys remain one of the most important modes of public transportation. However, commuters face several challenges:

1. **Fragmented Route Information**  
   - Jeepney routes are often informal and undocumented.  
   - Commuters rely on word-of-mouth, outdated maps, or social media posts.  
   - Tourists and new residents struggle to navigate efficiently.

2. **Event-Based Route Disruptions**  
   - During major city events like the MassKara Festival, elections, or road works, routes and stops change.  
   - Commuters cannot easily access real-time route adjustments.

3. **Fare Uncertainty**  
   - Fares vary by route, distance, and vehicle type, causing confusion.  
   - There is no centralized system to calculate or verify fares.

4. **Limited Local POI Awareness**  
   - Commuters and tourists have difficulty discovering nearby points of interest (restaurants, cafes, landmarks).  
   - Existing mapping platforms do not provide curated Bacolod-specific information.

5. **Data Decay**  
   - Routes, stops, and fare information may become outdated.  
   - No controlled mechanism exists for updating this data efficiently.

---

## Proposed Solution

The proposed system, **GoBacolod**, is a **web and mobile-based AI-assisted routing platform** that integrates MCP governance and RAG-powered intelligence to solve the above problems. Key solutions include:

1. **Centralized Jeepney Routes**  
   - Official routes from LPTRP and validated community updates are stored in a structured database.  
   - Routes are visualized on an interactive city map.

2. **Event Overlay Module**  
   - Government or authorized users can pin events (e.g., festivals, elections) on the map.  
   - The system dynamically adjusts route recommendations to account for closures, detours, and event-specific changes.

3. **AI-Assisted Navigation (RAG + MCP)**  
   - Commuters ask natural language questions (e.g., “How do I get from SM Bacolod to Lacson Street?”).  
   - AI retrieves structured route and POI data, ensures compliance via MCP, and responds with safe, context-aware directions.

4. **Crowdsourced Data Submission**  
   - Commuters can submit updated route suggestions or fare information.  
   - Submissions are moderated and approved by admins before integration to prevent errors.

5. **Fare Calculation System**  
   - Fare estimates are calculated automatically based on route distance and fare matrices.  
   - The AI provides verified, updated fare information to commuters.

6. **Points of Interest (POI) Recommendation**  
   - Local restaurants, landmarks, and attractions are stored with basic metadata (name, category, coordinates, optional image).  
   - AI recommends nearby POIs to commuters and tourists based on location queries.  
   - Optional external links for reviews can be provided without scraping or violating copyright.

7. **Developer-Facing Transport Data API**  
   - Third-party developers can access approved route, fare, and POI data.  
   - Enables integration into other apps while maintaining MCP governance and data integrity.

---

## Core Functions / Features

| Module | Functionality |
|--------|---------------|
| **Jeepney Routing** | Visualize routes, stops, and transfers; display distance and travel info. |
| **AI Assistant (RAG + MCP)** | Respond to natural language queries with verified, context-aware route guidance, fare info, and POI recommendations. |
| **Event Overlay** | Pin official events; dynamically update route suggestions during closures, festivals, or emergencies. |
| **Crowdsourced Data Submission** | Users submit route/fare updates; admins validate submissions before integration. |
| **Fare Calculation** | Estimate fare automatically based on route distance and predefined fare matrix. |
| **POI Recommendation** | Recommend nearby points of interest, including local restaurants, landmarks, and attractions. |
| **Developer API** | Expose approved route, fare, and POI data for external application integration. |

---

## Scope

1. Covers Bacolod City jeepney routes only.  
2. Includes natural language AI queries using RAG + MCP for context-aware navigation.  
3. Event overlay limited to official government or authorized admin events.  
4. POI database contains curated points of interest (restaurants, landmarks, public buildings).  
5. Crowdsourced submissions must undergo administrative approval before affecting system output.  
6. System supports mobile and web platforms.  
7. Developer API limited to approved route, fare, and POI data.

---

## Limitations

1. **Real-Time GPS Tracking**: Does not track jeepneys in real-time; relies on static or crowdsourced route data.  
2. **Review Data**: No live user reviews for POIs; optional external links only.  
3. **Fare System**: Does not cover all fare variations such as student or senior discounts unless manually updated.  
4. **Crowdsourcing Dependence**: Accuracy depends on user submissions and admin approval.  
5. **Internet Requirement**: Requires active internet connection to query AI and retrieve maps.  
6. **Limited Event Integration**: Only events entered by authorized users are considered; community-submitted events are not automatically included.  
7. **Scope**: Focused on Bacolod City; does not cover other transport modes (buses, tricycles) or neighboring cities.

---

## Expected Benefits

- **Commuters / Tourists**: Access accurate jeepney routes, fares, and POI recommendations; plan trips efficiently.  
- **Government / Admins**: Publish official events and ensure safe navigation; reduce commuter confusion.  
- **Developers**: Access curated transport data via API for integration into other apps.  
- **Overall City Mobility**: Encourages data-driven transport improvements and dynamic route management.

---

