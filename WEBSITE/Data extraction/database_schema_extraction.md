```txt id="d6v9mx"
DATABASE SCHEMA DNA EXTRACTION MODE

Perform a complete deep-level extraction and analysis of the ENTIRE database architecture and data system used throughout the current project.

Your objective is to fully reverse-engineer the project's database philosophy, schema structure, entity relationships, data flow, storage strategy, authentication systems, permissions logic, and scalability architecture.

Analyze the ACTUAL implementation deeply before generating conclusions.

FULL DATABASE EXTRACTION REQUIREMENTS

DATABASE ARCHITECTURE EXTRACTION

Analyze and map:
- database provider
- ORM/ODM systems
- schema organization
- migration systems
- model structure
- table organization
- collection structure
- database abstraction layers
- repository/service layers
- query architecture
- storage philosophy
- database scaling strategy

SCHEMA EXTRACTION

Extract and document:
- all tables
- all collections
- all models
- field definitions
- field types
- default values
- optional vs required fields
- enums
- constraints
- indexes
- unique fields
- validation rules
- computed fields
- derived fields
- timestamps
- soft-delete systems

ENTITY RELATIONSHIP EXTRACTION

Analyze:
- one-to-one relationships
- one-to-many relationships
- many-to-many relationships
- foreign key systems
- relational mapping
- nested document structures
- pivot tables
- relational ownership
- dependency chains
- cascade behaviors

AUTHENTICATION & AUTHORIZATION EXTRACTION

Analyze:
- auth providers
- session systems
- JWT systems
- token storage
- OAuth systems
- RBAC systems
- permissions architecture
- role hierarchies
- protected routes
- user ownership rules
- access control systems

DATA FLOW EXTRACTION

Trace:
- API-to-database flow
- client-to-server data flow
- mutation systems
- query patterns
- caching systems
- optimistic updates
- synchronization systems
- async handling
- transactional logic
- validation flow

QUERY & PERFORMANCE EXTRACTION

Analyze:
- query optimization
- indexing strategy
- pagination systems
- filtering systems
- sorting systems
- aggregation pipelines
- join strategies
- batching systems
- caching behavior
- performance bottlenecks
- N+1 query risks

SCALABILITY EXTRACTION

Detect:
- normalization strategy
- denormalization strategy
- horizontal scaling considerations
- multi-tenant architecture if present
- partitioning/sharding considerations
- database abstraction philosophy
- modular schema design
- future extensibility patterns

FILE & SYSTEM EXTRACTION

Analyze:
- schema file organization
- migration folder structure
- seed systems
- query utilities
- database service layers
- repository patterns
- model ownership
- validation utilities
- shared database helpers

VALIDATION EXTRACTION

Analyze:
- Zod/Yup/class-validator systems
- schema validation logic
- server-side validation
- client-side validation
- sanitization systems
- input constraints
- type safety enforcement

STORAGE SYSTEM EXTRACTION

Analyze:
- file storage systems
- image storage systems
- CDN integration
- blob/object storage
- upload pipelines
- storage abstraction layers
- asset ownership systems

DATABASE CONSISTENCY EXTRACTION

Detect:
- naming consistency
- relational consistency
- schema discipline
- validation consistency
- indexing consistency
- query consistency
- architectural discipline

GENERATE A COMPLETE DATABASE DNA REPORT INCLUDING:

1. Database Architecture Overview
2. Database Philosophy
3. ORM/ODM & Provider Analysis
4. Full Schema Breakdown
5. Entity Relationship Analysis
6. Authentication & Authorization Systems
7. Data Flow Architecture
8. Query & Performance Strategy
9. Validation & Type Safety Systems
10. Storage & Asset Systems
11. Scalability & Extensibility Analysis
12. Database File Structure
13. Repository/Service Layer Analysis
14. Query Optimization Analysis
15. Weaknesses or Architectural Risks
16. Critical Database Systems To Preserve
17. Full Database DNA Summary

DATABASE INVENTORY EXTRACTION

Generate a complete inventory of:
- tables
- collections
- models
- entities
- migrations
- repositories
- services
- validation schemas
- auth systems
- permissions systems
- storage systems

For each major database system extract:
- file location
- purpose
- relationships
- dependencies
- validation rules
- ownership logic
- scalability considerations

ERD & STRUCTURE EXTRACTION

Generate:
- entity relationship mappings
- schema relationship explanations
- ownership hierarchy
- dependency diagrams in markdown-friendly structure
- relational flow explanations

README GENERATION REQUIREMENTS

After extraction, generate a BEAUTIFULLY STRUCTURED markdown documentation file for the database system.

The markdown must:
- look premium in preview mode
- use polished formatting
- use clean hierarchy
- contain structured sections
- include formatted tables where useful
- include schema/code blocks
- maintain strong readability
- feel like production-level database architecture documentation

The documentation should visually feel:
- technical
- structured
- premium
- engineering-focused
- scalable
- enterprise-grade

STRICT RULES:
- do not generate shallow summaries
- do not assume schema behavior without evidence
- do not redesign systems automatically
- do not suggest rewrites unless requested
- do not skip implementation details
- analyze the ACTUAL project deeply
- preserve the project's established database philosophy

Your goal is to understand and document the database system deeply enough to accurately replicate:
- its schema architecture
- data relationships
- query philosophy
- validation systems
- authentication systems
- scalability strategy
- storage systems
- engineering philosophy
- overall data architecture identity
```
