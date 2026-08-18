🏗️ Bharat Rakshak — Technical Design
1. System Architecture
Bharat Rakshak uses an offline-first, local-data architecture.
┌──────────────────────┐
│        USER          │
│   Explore / Search   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│      FRONTEND        │
│    HTML / CSS / JS   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│    CONTENT LOGIC     │
│ Search • Filters     │
│ Profiles • Categories│
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│      LOCAL DATA      │
│    JSON / Records    │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│       STORAGE        │
│     LocalStorage     │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│       OUTPUT         │
│       Results        │
└──────────────────────┘
2. Architecture Principles
Offline First: Core reference content should remain accessible without continuous internet.
Local First: Primary reference information is held in local records.
Simple: Lightweight frontend architecture.
Searchable: Search, filters and categories support discovery.
Multilingual: English plus nine Indian languages in the prototype.
Privacy Conscious: Local-first approach with no unnecessary tracking.
3. Main Components
Frontend
HTML + CSS + JavaScript
Responsibilities:
Dashboard.
Navigation.
Search interface.
Filters.
Profiles.
Categories.
Language settings.
Results display.
Content Logic
Responsibilities:
Search records.
Apply filters.
Load profiles.
Handle categories.
Process user interactions.
Display results.
Local Data
Structured JSON/records represent:
Wars.
Battles.
Operations.
Heroes.
Martyrs.
Gallantry awards.
Quotes.
Regimental heritage.
Storage
LocalStorage provides client-side local persistence where required.
4. Conceptual Data Design
Local Data
│
├── Wars
│   ├── War information
│   ├── Operations
│   ├── Chronology
│   ├── Theatre
│   └── Outcomes
│
├── Heroes / Martyrs
│   ├── Profile information
│   ├── Service information
│   └── Source / verification status
│
├── Gallantry Awards
│   ├── Award
│   ├── Category
│   ├── Recipient
│   └── Citation
│
├── Quotes
│   ├── Quote
│   ├── Attribution
│   └── Context
│
└── Regimental Heritage
    └── Historical information
This is the conceptual organization of the project's local data, rather than a claim of a separate remote database.
5. Search and Filtering
User Query
    ↓
Search / Filter Logic
    ↓
Local Records
    ↓
Matching Results
    ↓
Profile / Information View
Search and filters operate against the local reference records.
6. Multilingual Design
The prototype provides:
English + 9 Indian languages
Conceptual flow:
User selects language
        ↓
Language setting
        ↓
Localized UI content
        ↓
Updated interface
The localization structure should remain extensible so additional languages can be added later.
7. Offline Design
The primary reference experience does not depend on external APIs.
USER
  ↓
FRONTEND
  ↓
CONTENT LOGIC
  ↓
LOCAL DATA
  ↓
LOCAL STORAGE
  ↓
RESULTS
The network is not required for the core local reference flow.
8. API Design
Current Prototype
The core reference experience is designed without external API dependency.
Primary Reference Experience
          ↓
Local JSON / Records
          ↓
LocalStorage
          ↓
Application
Future Possibility
Optional secure update/import mechanisms may be added in future versions while preserving offline access.
No external API is claimed as part of the current core prototype unless separately implemented.
9. AI / Kiro Development Layer
Amazon Kiro is part of the development process:
Idea
  ↓
Requirements
  ↓
Kiro Spec
  ↓
Design
  ↓
Tasks
  ↓
AI Agent
  ↓
Implementation
  ↓
Testing
  ↓
Iteration
Kiro was used to structure requirements and tasks and to assist with implementation and refinement.
10. Component Communication
USER
 │
 ▼
FRONTEND
 │
 ▼
CONTENT LOGIC
 │
 ├── Search
 ├── Filters
 ├── Profiles
 └── Categories
 │
 ▼
LOCAL DATA
 │
 ▼
LOCAL STORAGE
 │
 ▼
OUTPUT
11. Security / Privacy Principles
The design emphasizes:
Local-first access.
Offline functionality.
No unnecessary tracking.
Reduced dependency on external services.
Historical and military information should be reviewed by humans before being treated as verified information.
12. Future Technical Scope
Potential improvements:
Larger verified personnel database.
Advanced timelines.
Interactive maps.
Battle visualisations.
Improved source management.
Editorial verification workflows.
Secure update/import mechanisms.
Accessibility improvements.
Educational modules.
PWA/installable offline application.
13. Technical Summary
User → HTML/CSS/JS Frontend → Content Logic → JSON/Records → LocalStorage → Results
This architecture keeps Bharat Rakshak lightweight, searchable and offline-first.
