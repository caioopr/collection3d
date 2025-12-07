# Collection3D — Software Requirements Specification (SRS) - v0.1.1
# Table of Contents
- [[#1. Summary]]
- [[#2. Introduction]]
	- [[#2.1 Purpose]]
	- [[#2.2 Document Conventions]]
	- [[#2.3 Intended Audience]]
	- [[#2.4 Scope]]
	- [[#2.5 References]]
- [[#3. Glossary]]
- [[# 4. Actors]]
- [[#5. User Stories]]
- [[#6. Use Cases]]
	- [[#6.1 Use Case Diagram]]
	- [[#6.2 Use Case Descriptions]]
- [[#7. Functional Requirements (FRs)]]
- [[#8. Non-Functional Requirements (NFRs)]]
	- [[#8.1 Performance]]
	- [[#8.2 Security]]
	- [[#8.3 Usability]]
	- [[#8.4 Reliability & Availability]]
	- [[#8.5 Maintainability & Scalability]]
- [[#9. User Interface & UX]]
	- [[#9.1 UI Flow]]
	- [[#9.2 Wireframes / Prototypes]]
- [[#10. System Architecture]]
	- [[#10.1 Logical View]]
	- [[#10.2 Process View]]
	- [[#10.3 Development View]]
	- [[#10.4 Data View]]
	- [[#10.5 Physical View]]
- [[#11. Database Design]]
	- [[#11.1 ER Diagram]]
	- [[#11.2 Entity Definitions]]
	- [[#11.3 Normalization Notes]]
- [[#12. API Design]]
	- [[#12.1 Overview]]
	- [[#12.2 OpenAPI Specification (external file)]]
	- [[#12.3 Endpoints Summary]]
- [[#13. Tools & Technologies]]
- [[#14. Contribution Guidelines & Standards]]
- [[#15. Revision History]]
---
## 1. Summary
Collection3D is a web-based platform for uploading, managing, visualizing, and sharing 3D models files.
The system allows users to maintain a personal library of 3D assets while also contributing to a public community space where models can be explored by anyone.

This Software Requirements Specification (SRS) defines the functional and non-functional requirements, personas, use cases, data models, system architecture, and API design necessary to guide the development of Collection3D.
It serves as the single source of truth across all milestones, ensuring consistent implementation across frontend, backend, testing, and documentation efforts.

This document also supports long-term maintainability by providing traceability between requirements, user stories, use cases, data models, and API definitions.
---
## 2. Introduction
### 2.1 Purpose
The purpose of this document is to formally specify all requirements for the Collection3D platform, including functional behavior, non-functional expectations, architectural constraints, and interface definitions.
It provides a shared understanding for developers, designers, testers, and future contributors by serving as the authoritative reference throughout all development milestones.

### 2.2 Document Conventions
This document follows the conventions below:

**Requirement Labels**
- ***FR-n***: Functional Requirement  
- ***NFR-n***: Non-Functional Requirement  
- ***UC-n***: Use Case  
- ***US-n***: User Story

**Modal Verbs**
- ***Shall / Must***: Indicates a mandatory requirement  
- ***Should***: Indicates a recommended but not mandatory behavior  
- ***May***: Indicates an optional feature or behavior

**Formatting Rules**
- Technical names such as database fields, DTO attributes, and API endpoints are written in `monospace`.

### 2.3 Intended Audience
This document is intended for:
- Developers (Frontend & Backend): to implement features consistently
- Designers: to design UI elements aligned with system behavior
- Test Engineers: to define acceptance criteria and test cases
- Project Maintainers: to track changes and maintain documentation
- Contributors: to understand architecture, coding standards, and requirements prior to contributing

### 2.4 Scope
The scope covers the Minumum Viable Product(MVP) and near-future milestones required to support model management, visualization, and community-driven content discovery.

The platform MVP provides:
- A secure authentication system for account creation and management
- A user dashboard for managing personal 3D models.
- A public “Community Models” gallery for browsing shared assets.
- A full 3D viewer supporting 3D mesh files rendering.
- APIs for uploading, deleting, updating, and retrieving 3D files and metadata.
- A well-structured backend written in Go (using the standard library + Gorilla Mux).
- A PostgreSQL database managed via SQLC for safe, type-checked queries.
- A frontend built with Nuxt.js for a fast, modern user experience.

### 2.5 References
---
## 3. Glossary
| Term | Definition |
|------|------------|
| **API (Application Programming Interface)** | The HTTP interface exposed by the backend for client communication. |
| **Asset** | A generic term for any uploaded file (3D model, thumbnail, metadata). |
| **Authenticated User** | A user who has completed the sign-in flow and has a valid session/token. |
| **Community Models** | Publicly visible 3D models contributed by users and available for all visitors. |
| **DTO (Data Transfer Object)** | A structured object used to exchange data between frontend, backend, and API layers. |
| **FR (Functional Requirement)** | A specification describing behavior the system must implement. |
| **GLB** | A binary version of the GLTF format, bundling geometry, materials, textures, and scene data. |
| **GLTF** | A specification for efficient transmission of 3D scenes and models, often referencing external resources. |
| **Material** | Visual properties applied to a mesh, such as color, roughness, or textures. |
| **Mesh** | The collection of vertices, edges, and faces that define the shape of a 3D object. |
| **NFR (Non-Functional Requirement)** | A specification describing performance, security, reliability, or other quality attributes. |
| **SQLC** | A tool for generating type-safe Go code from SQL queries. |
| **Texture** | An image used to add detail to a 3D model’s surface. |
| **3D Model** | A digital asset representing a three-dimensional object, stored in formats such as GLB or GLTF. |
| **UC (Use Case)** | A detailed interaction between an actor and the system to achieve a goal. |
| **US (User Story)** | A story capturing a requirement from the perspective of a user. |
| **User** | Any authenticated or unauthenticated individual interacting with the system. |
| **Viewer** | The interactive component responsible for rendering 3D models allowing user interaction. |

---
## 4. Actors
---
## 5. User Stories
---
## 6. Use Cases
### 6.1 Use Case Diagram
### 6.2 Use Case Descriptions
---
## 7. Functional Requirements (FRs)
---
## 8. Non-Functional Requirements (NFRs)
### 8.1 Performance
### 8.2 Security
### 8.3 Usability
### 8.4 Reliability & Availability
### 8.5 Maintainability & Scalability
---
## 9. User Interface & UX
### 9.1 UI Flow
### 9.2 Wireframes / Prototypes
---
## 10. System Architecture
### 10.1 Logical View
### 10.2 Process View
### 10.3 Development View
### 10.4 Data View
### 10.5 Physical View
---
## 11. Database Design
### 11.1 ER Diagram
### 11.2 Entity Definitions
### 11.3 Normalization Notes
---
## 12. API Design
### 12.1 Overview
### 12.2 OpenAPI Specification (external file)
### 12.3 Endpoints Summary
---
## 13. Tools & Technologies
---
## 14. Contribution Guidelines & Standards
---
## 15. Revision History
| Version | Date       | Author | Description |
|---------|------------|--------|-------------|
| 0.1.0   | 2025-12-06 | Caio Prado | Initial draft of the SRS document created. |
| 0.1.1   | 2025-12-07 | Caio Prado | Added Summary, Introduction, and Glossary sections. |