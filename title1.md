# GoBacolod: An MCP-Governed AI-Assisted Jeepney Routing and Safe Navigation System for Bacolod City

## 1. Problem Statement

Public transportation in Bacolod City relies heavily on jeepneys, yet there is no centralized, structured, and accessible digital system for jeepney routing. Existing route information is often:

- Scattered across unofficial maps and social media posts  
- Based on outdated LPTRP documents  
- Not available in structured API format  
- Difficult for new commuters and students to understand  

Mainstream navigation platforms such as Google Maps do not accurately represent jeepney route logic, loop systems, and designated stops within Bacolod City. As a result:

- Commuters experience confusion in selecting correct routes  
- New residents and visitors struggle with local transportation  
- Developers lack access to standardized jeepney routing data  
- There is no AI-driven system that explains routes in a localized, conversational manner  

Therefore, there is a need for a structured, AI-assisted, and MCP-governed jeepney routing system that provides accurate route retrieval, safe navigation guidance, and controlled AI tool access for Bacolod City.

---

## 2. Project Scope

### 2.1 Geographic Scope

- Coverage limited to Bacolod City  
- Based on officially issued LPTRP jeepney routes  
- Static route data (no real-time GPS tracking)

---

### 2.2 Functional Scope (User-Facing System)

The system will:

1. Provide a digital map interface displaying jeepney route polylines  
2. Allow users to input origin and destination points  
3. Retrieve appropriate jeepney routes based on structured database queries  
4. Extract route segments between selected locations  
5. Identify nearest jeepney stops  
6. Provide AI-generated route explanations using retrieved data  
7. Support safe navigation by optionally overlaying hazard-prone areas (if available)  
8. Implement MCP governance to control how the AI accesses routing tools  

The system will use Retrieval-Augmented Generation (RAG) to ensure the AI assistant generates responses based only on verified route data.

---

### 2.3 System Architecture Scope

The system will include:

- A jeepney route database  
- A routing logic module  
- An AI assistant interface  
- An MCP server to manage tool execution  
- REST-based internal APIs for route and stop retrieval  

---

### 2.4 Excluded Features (Limitations)

The system will NOT include:

- Real-time jeepney GPS tracking  
- Dynamic traffic-based rerouting  
- Fare computation engine  
- Payment integration  
- Multi-city support  
- Multi-transfer route optimization  

These features are considered future enhancements beyond the scope of this study.

---

## 3. Primary Beneficiaries

### 3.1 Community Residents of Bacolod City

- Daily commuters  
- Students  
- Workers  
- New residents  

Benefits:
- Clear and structured jeepney route guidance  
- Reduced confusion in loop-based routes  
- Faster and safer route planning  
- Conversational AI assistance tailored to local transport  

---

### 3.2 Local Developers and Technology Innovators

Benefits:
- Access to structured jeepney route data  
- Potential integration of routing data into third-party applications  
- Standardized format for mobility-related system development  
- Foundation for future smart city applications  

---

## 4. Expected Contribution

GoBacolod contributes to:

- Digitization of local public transportation routes  
- Controlled AI tool integration using MCP  
- RAG-based mobility assistance  
- Smart mobility infrastructure development for Bacolod City  
- Foundational transport data standardization  

This project aims to provide both a practical navigation solution for commuters and a technical framework for AI-governed public transport systems.
