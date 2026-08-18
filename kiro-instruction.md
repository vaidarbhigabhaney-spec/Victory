🤖 Bharat Rakshak — Instructions Given to Amazon Kiro
Project Identity
Project: Bharat Rakshak — भारत रक्षक
Tagline: Preserve • Remember • Educate
Team: Victory
College: Ratan Tata Maharashtra State Skills University, Nagpur
Event: Amazon Kiro Buildathon
1. Master Project Instruction
Build Bharat Rakshak, a digital heritage portal for India's Armed Forces.
The application should provide a structured, searchable, multilingual and offline-first experience for exploring:
India's wars.
Battles and operations.
Martyrs and heroes.
Gallantry award recipients.
Military heritage.
Attributed historical quotes.
The application must be simple, fast, respectful and easy to navigate.
2. Critical Requirement — Offline First
The most important technical requirement is:
The core reference experience must work without internet connectivity.
Do not make the primary reference experience dependent on external APIs.
Use local structured data such as:
JSON.
Local records.
LocalStorage.
Avoid unnecessary network requests.
3. Target Users
Design for:
Students.
Citizens.
Researchers.
Defence enthusiasts.
The application should be understandable to general users while keeping the information structured enough for educational and research use.
4. Frontend
Use:
HTML.
CSS.
JavaScript.
Create a responsive interface suitable for mobile and desktop.
Prioritize:
Readability → Navigation → Information → Visual design
5. Main Sections
Create the following major sections:
Dashboard
├── Wars & Battles
├── Martyrs & Heroes
├── Gallantry Awards
├── Quote Explorer
├── Regimental Heritage
└── Settings / Language
6. Dashboard
Create a dashboard for quick access to the main sections.
Display major categories such as:
Wars.
Martyrs.
Gallantry Awards.
Heroes & History.
Use the project branding:
BHARAT RAKSHAK
भारत रक्षक
Preserve • Remember • Educate
7. Wars & Battles
Create a structured section for wars, battles and operations.
Support information such as:
Name.
Date/period.
Operation.
Theatre.
Description.
Outcome.
Related historical information.
Provide search, filters and detailed views.
8. Martyrs & Heroes
Create structured profiles for martyrs and heroes.
Where available, support:
Name.
Service information.
Unit/regimental information.
Historical context.
Service/sacrifice information.
Related awards.
Source/verification status.
Do not invent missing information.
9. Gallantry Awards
Create a section for gallantry awards.
Support:
Award name.
Award category.
Recipient.
Citation.
Historical context.
Source/verification status.
Allow browsing and searching.
10. Quote Explorer
Create a quote-discovery section.
Requirements:
Show attributed quotes.
Provide context where available.
Display attribution.
Support random quote discovery.
Do not present unverified quotations as confirmed facts.
11. Multilingual UI
The prototype should support:
English + 9 Indian languages
Create a language-selection mechanism.
Keep localization modular so additional Indian languages can be added later.
Do not hardcode every language string into unrelated components.
12. Local Data
Use structured local data.
Conceptually organize records around:
Wars
Heroes
Martyrs
Awards
Quotes
Regimental Heritage
A possible structure is:
data/
├── wars.json
├── heroes.json
├── martyrs.json
├── awards.json
├── quotes.json
└── regiments.json
Use an implementation structure that remains modular and maintainable.
13. Storage
Use LocalStorage for appropriate client-side persistence.
Do not require a remote database for the primary offline reference experience.
14. Search and Filters
Implement reusable search/filter functionality.
Examples of searches include:
Award name.
War.
Year.
Service.
Hero/martyr name.
Battle or operation.
Filters should be relevant to the selected category.
15. Historical Accuracy
Military and historical information must be treated carefully.
Rules:
Never invent historical facts.
Never fabricate names.
Never fabricate award citations.
Never fabricate dates.
Preserve source/verification information where available.
Clearly identify information requiring review.
Human review is required for historical facts and sensitive military information.
16. UI and Visual Design
Create a respectful patriotic visual identity.
The interface should communicate:
Heritage.
Respect.
Education.
Remembrance.
Do not make the interface unnecessarily complicated.
17. Performance
The application should:
Load quickly.
Minimize unnecessary dependencies.
Work efficiently with local data.
Avoid unnecessary network requests.
Remain usable offline.
18. Privacy
Use a local-first approach.
Do not add unnecessary tracking or third-party analytics.
19. Kiro Specification Workflow
Develop the project using this workflow:
IDEA
 ↓
REQUIREMENTS
 ↓
KIRO SPEC
 ↓
DESIGN
 ↓
TASKS
 ↓
AI AGENT
 ↓
IMPLEMENTATION
 ↓
TESTING
 ↓
REVIEW
 ↓
ITERATION
Do not simply generate the entire project in one step.
Break requirements into specifications and tasks that can be implemented and tested independently.
20. Feature Development Process
Before implementing each major feature:
Understand the requirement.
Define expected behavior.
Define acceptance criteria.
Identify required data.
Design the UI.
Break the feature into tasks.
Implement the tasks.
Test the feature.
Review the result.
Fix issues and iterate.
21. Implementation Priority
Implement in this order:
Phase 1
Project structure and base UI.
Phase 2
Dashboard.
Phase 3
Wars & Battles.
Phase 4
Martyrs & Heroes.
Phase 5
Gallantry Awards.
Phase 6
Quote Explorer.
Phase 7
Search and Filters.
Phase 8
Multilingual UI.
Phase 9
Offline/local storage.
Phase 10
Testing and refinement.
22. Testing Instructions
Test:
Navigation
Every main section must open correctly.
Search
Search must return matching local records.
Filters
Filters must correctly narrow results.
Profiles
Profiles must display their available information correctly.
Language
Language selection must update supported interface text.
Offline
Disable network access and verify that the core reference experience continues to work.
Responsive UI
Test mobile, tablet and desktop layouts.
23. Error Handling
If information does not exist:
"No matching information found."
Do not create fictional historical information to fill an empty result.
24. Acceptance Criteria
The application is successful when:
Bharat Rakshak is functional.
Main navigation works.
Wars and battles can be explored.
Martyrs and heroes can be explored.
Gallantry awards can be explored.
Quotes can be discovered.
Search and filters work.
Multilingual interface is available.
Core reference content works offline.
Local data supports the primary reference experience.
The UI is responsive and easy to use.
Historical information is handled with verification awareness.
25. Future-Compatible Design
Keep the application modular enough to support future:
Larger verified personnel database.
Advanced timelines.
Maps.
Battle visualisations.
Source-management systems.
Editorial verification workflows.
Secure data update/import.
Educational modules.
Accessibility improvements.
PWA/installable offline functionality.
Future functionality must not become a dependency for the current prototype.
26. Final Kiro Instruction
Build Bharat Rakshak as a complete, respectful, fast, accessible and offline-first digital heritage portal.
Prioritize:
Correctness.
Offline functionality.
Simplicity.
Searchability.
Accessibility.
Maintainability.
Human verification of historical information.
Use Amazon Kiro's specification-driven workflow throughout development and keep the implementation traceable to the project requirements.
Preserve • Remember • Educate
