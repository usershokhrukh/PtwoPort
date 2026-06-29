Logo : ![logo](<img src="./public/logo/logo-fill.svg" width="48">)
#+html: <img src="./public/logo/logo-fill.svg" width="48">

# 🚀 PtwoPort — Visual Mock API Generator

**PtwoPort** — dasturchilar uchun backend kodini qoʻlda yozmasdan, vizual tarzda **Mock API** endpointlarini chizish imkonini beruvchi SaaS platformadir. Barcha ma'lumotlar foydalanuvchining shaxsiy kompyuteridagi `db.json` fayliga real vaqtda yozib boriladi!

---

## 🎨 1. Arxitektura (2-Part Architecture)

Brauzer sandbox cheklovlari tufayli lokal fayllarga to'g'ridan-to'g'ri yoza olmaydi. Shu sababli tizim ikki qismdan iborat:
1. **Brauzer UI (SaaS):** Faqat dizayn va visual boshqaruv oynasi.
2. **Lokal CLI Agent (`npx ptwoport`):** Kompyuterda `4000-port`da Mock API serverni ko'taradi va `db.json` faylini boshqaradi. UI bilan **WebSocket (WS)** orqali bog'lanadi.

---

## 🛡️ 2. Xavfsizlik va Maxfiylik

* **100% Maxfiylik:** Ma'lumotlaringiz hech qanday bulutli (Cloud) serverga chiqmaydi, hammasi o'zingizning kompyuterizda (`localhost`) qoladi.
* **Zero Installation:** Kompyuterga og'ir dasturlar o'rnatish shart emas, yadro fonda `npx` orqali vaqtincha ishga tushadi.

---

## 🚀 3. Tezkor Ishga Tushirish

1. **Yadroni yoqing:** Loyiha papkangizda terminalni ochib, buyruqni bering:
   ```bash
   npx ptwoport






## PtwoPort: Complete System Architecture & Deep Feature Specification
1. Introduction, Product Philosophy & Overall Purpose
PtwoPort is a developer tool designed as a Visual API Sandbox & Code Generator. It runs natively
on the user's local machine, providing frontend and mobile engineers with a rapid prototyping suite.
The core philosophy is to remove the friction of manual configuration required by traditional packages
like json-server and json-server-auth.
In modern software development, frontend engineers are often blocked while waiting for backend
teams to ship final APIs. While local mock servers solve this, traditional tools require setting up
dependencies, managing complex local database mock files, and manually implementing routing and
authorization logic. PtwoPort collapses these tasks into a unified graphical desktop application powered
by an isolated backend orchestration agent.
Core Product Objectives:

• Zero-Dependency Setup: Eliminate manual npm/pip installations for local server mocking.

• Visual Data Engineering: Provide a database-like visual interface to design structural,
relational JSON schema schemas instantly.

• Real-time Local Serving: Act as a hot-reloading mock engine that processes true HTTP
requests from applications, tools like Postman, or browsers.

• Production Code Blueprinting: Transition fluidly from a mock prototype to an enterprisegrade backend infrastructure by compiling visual trees into functional codebase files.

2. Deep-Dive Feature Specifications
⚙️ A. The Orchestration Engine (The Core Core)
The Engine is the background execution layer of PtwoPort. It operates as an isolated server agent using
Node.js or a localized multi-thread runner within an Electron environment.
Technical Execution Mechanics:

• Dynamic HTTP Virtualization: When a repository is active, the engine provisions a local
HTTP web server on a designated port (e.g., localhost:4000). It listens to raw inbound
TCP/IP connections.

• Schema Schema Translation: The Engine monitors the central state management
configuration file (.ptwoport). When a request lands, the engine acts as an interpreter: it
reads the request path, matches it to the configuration schema, dynamically injects contextual
mock properties, and serves an arrayed or object-based JSON payload.

• Hot-Reload Compilation: Every modification made within the user interface emits an InterProcess Communication (IPC) signal to the engine. The engine applies the modifications
directly to the memory stack and soft-restarts the network socket in under 200 milliseconds,
ensuring zero downtime for the frontend app listening to it.

 B. The Local Repository System
The Local Repository System handles data isolation, sandboxing, and local system state management.
Architectural Components:

• Isolated Workspace Directory: Creating a repository allocates an explicit project context
inside PtwoPort's memory space and generates a state marker called .ptwoport. This isolates
schema assets, ports, and data records between completely distinct applications (e.g., separating
an E-Commerce API from a ride-sharing API).

• Schema Snapshotting & Version Control: The engine tracks schema definitions
incrementally. When a user executes a snapshot ("Commit"), the core captures the precise
structure of the state tree. This creates a directional acyclic graph (DAG), enabling developers
to check out previous states, view schema mutations, or split testing implementations into
concurrent paths ("Branches") without corrupting their stable mock environment.
 C. Native Authentication System (json-server-auth Architecture)
PtwoPort replaces explicit authorization middleware logic with a native, declarative security layer.
Implementation Matrix:

• Automated Identity Endpoints: Toggling the global authentication layer prompts the engine to
reserve /login and /register routing mechanisms. These entry points intercept inbound
requests, parse input attributes, apply secure internal password hashing schemes, and sign out
standards-compliant JSON Web Tokens (JWTs).

• Granular Gatekeeping (Route Guards): Each endpoint row features an explicit authorization
lock. When enabled, the engine evaluates inbound request metadata for valid
Authorization: Bearer <token> headers before resolving the controller logic.
Requests failing verification are immediately dropped with a structured 401 Unauthorized
HTTP response.

• Identity Mapping Matrix: The data grid includes a native Logged-in User ID variable
modifier. When an authenticated client makes a payload-mutation request (such as POST
/orders), the engine extracts the cryptographic subject string from the token and maps it
automatically to the resource entry, guaranteeing true multitenancy simulation.
 D. Action Lab Terminal & Live Traffic Monitor
The lower dashboard houses an interactive Command-Line Interface (CLI) coupled with a real-time
event streaming pipeline.
Functional Specifications:

• Structured Stream Injection: The terminal acts as a structured debugger. Every socket
connection hitting the orchestration engine is captured, transformed into a standard access log
string, colorized by HTTP verb type, and streamed directly into the viewport console (e.g.,
[20:35:00] POST /api/v1/orders - 201 Created).

• Headless Shell Commands: To cater to advanced users, the terminal reads incoming string
sequences to manipulate app state without requiring user interaction with the graphical canvas:

• clear: Resets the live event stream viewport logs.

• restart: Triggers an explicit network socket recycle on the active endpoint pool.

• add [path]: Instructs the engine to spin up a baseline endpoint schema at the chosen
path immediately.

 E. Visual JSON Tree Editor (Endpoints Workspace)
The central matrix converts flat database schemas into nested JSON representations.
Data Formatting Capabilities:

• Typing Matrix: Supports explicit typing declarations including string, number, boolean,
array, object, and unique key entities (id).

• Dynamic Mock Integration (Auto-Faker): Integrates declarative structural templates directly
into data rows. Instead of assigning a static value, users can assign semantic patterns like
Faker.Name, Faker.Email, Faker.Image, or Faker.Currency. The underlying
runtime parses these directives and injects randomized, contextually valid strings on every
request execution.

3. Production Code Generation & Ecosystem
 Blueprint Compilation Engine
Once a developer finishes prototyping locally, they use the compilation suite located on the right side
panel to transition to production.

• Production Translation Pipeline: Clicking the execution action parsing engine recursively
loops through the configurations saved inside the .ptwoport file. It reads every declared
route path, permission level, relationship mapping, and data format model.

• Standalone Code Output: The engine translates these nodes into an organized structure
containing full production code (such as an Express.js or FastAPI application). This logic is
packaged directly into a local .zip file containing standard directory structures, controller
abstractions, dependency lists (package.json), routing models, and automated JWT
middleware configurations.

 4. Global Interface Grid Layout Map
The main viewport is organized using a zero-scroll application layout split into distinct system
windows:

+----------------------------------------------------------------------------------
--+
| 🌐 NAVBAR: Workspace Selector | Global Search Input | Agent Status | User Profile
|
+------------------------------------
+-----------------------------------------------+
| LEFT SIDEBAR | CENTER WORK BOARD (Visual JSON Editor) |
| |
|
| - Projects Dropdown | - Route Header: [POST] /api/v1/orders
|
| - Commit & Branch: [main ] | - View Toggle: [Editor] / [Documentation] ▾
|
| - API Collections (Folders)
+-----------------------------------------------+
| - Endpoint Items with Method Tags | | Key | Type | Default |
|
| [GET] /users | | customer_name | Faker.Name | - |
|
| [POST] /orders [ Protected] | | total_price | number | 0 |
|
| |
+-----------------------------------------------+
| - Quick Add Button (+) | BOTTOM TERMINAL (Action Lab)
|
| | - [20:35:00] POST /api/v1/orders - 201
Created|
| | - ptwoport> _ (Command line: clear, restart)
|
+------------------------------------
+-----------------------------------------------+
| RIGHT SIDEBAR (Code Integration & Export)
|
| - Snippet Tabs: [JavaScript] [Python] [cURL]
|
| - Copyable Axios/Fetch code block
|
| - Action: [Share Schema via Link]
|
| - Action: [Export Code (.zip) - Express.js/FastAPI Generator]
|
+----------------------------------------------------------------------------------
--+

5. Software Licensing & Intellectual Property Integrity
A key design aspect of PtwoPort is its complete independence from third-party ecosystems during
execution. While it replaces the utility of traditional tools like json-server and json-serverauth, it avoids open-source compliance or commercial licensing complications.
Legal & Open-Source Architecture Analysis:

• Permissive Licensing Compliance: Popular command-line mock utilities typically operate
under highly permissive open-source models, such as the MIT License. This explicit grant
allows anyone to study the architectural behavior, modify the execution concepts, or engineer
completely new, independent solutions that solve similar software delivery bottlenecks.

• Clean-Room Software Engineering: PtwoPort is built entirely on a clean-room software
development framework. It does not inherit, fork, or copy internal source code files from
external libraries. Instead, its underlying orchestration agent is built entirely from scratch using
separate internal network protocols, graphical abstractions, and serialization formatting logic.

• Zero Proprietary Infringement: Developers have full ownership over their engineered
projects. Because the application logic executes natively on a completely offline workstation
without injecting or distributing proprietary runtime assets, it is fully compliant with opensource distribution frameworks and commercial development standards.