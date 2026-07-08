# Software Design Studio — TODO

## Phase 1: Database Schema & Backend

- [x] Design and write Drizzle schema: projects, requirements, arch_components, test_cases, traceability_links, audit_log
- [x] Generate and apply DB migrations
- [x] tRPC router: projects (CRUD)
- [x] tRPC router: requirements (CRUD, status transitions, unique ID generation)
- [x] tRPC router: arch_components (CRUD, link to requirements)
- [x] tRPC router: test_cases (CRUD, link to requirements + components)
- [x] tRPC router: traceability (matrix query, coverage stats)
- [x] tRPC router: validation (rule engine — completeness, naming, coverage)
- [x] tRPC router: reports (coverage metrics, audit trail)
- [x] tRPC router: ai_assist (LLM-backed drafting for reqs, arch notes, test cases)

## Phase 2: Frontend Layout & Navigation

- [x] Global CSS theme — dark professional palette, refined typography (Inter/JetBrains Mono)
- [x] WorkbenchLayout sidebar with navigation: Requirements, Architecture, Code, Tests, Reports, Validation, Timeline
- [x] Project selector / switcher in sidebar header
- [x] Pipeline status bar: Reqs → Arch → Code → Tests → Reports with phase indicators
- [x] Dashboard home page with project overview and pipeline status cards

## Phase 3: Requirements Module

- [x] Requirements chatbot page with AI conversation interface
- [x] Datasheet upload (PDF) with LLM extraction
- [x] Module/MCU chip input panel
- [x] Generated TODO list with sync to requirements
- [x] Status badge: Draft / Review / Approved
- [x] Requirements list tab with formal REQ-XXXX entries

## Phase 4: Architecture Module

- [x] STM32F407 graphical pin map (64-pin LQFP SVG, clickable pins)
- [x] Pin color coding by function (Input/Output/Alternate/Analog/Power/NC)
- [x] Pin settings modal (mode, function, label, notes)
- [x] Schematic PDF upload with AI extraction
- [x] AI Auto-Config from project context
- [x] Components tab with CRUD
- [x] Traceability matrix tab

## Phase 5: Code IDE Module

- [x] Multi-file tree sidebar (main.c, drivers/, Inc/, Src/ structure)
- [x] CodeMirror-based code editor (C syntax highlighting)
- [x] Graphical PLC-like block editor (SVG canvas with drag-and-drop blocks)
- [x] Toggle between Code view and Graphical view (same context)
- [x] AI Code Assistant panel (right sidebar with change messages)
- [x] Generate Skeleton from requirements
- [x] Block types: Init, Loop, Condition, GPIO, UART, Delay, Function Call

## Phase 6: Tests Module

- [x] Test case list page with filters (unit/integration, pass/fail/pending)
- [x] Test case creation form (title, type, steps, expected result, status, linked requirement, linked component)
- [x] Test status tracking: Pending / Pass / Fail / Blocked
- [x] Test-to-requirement traceability display

## Phase 7: Validation Engine

- [x] Validation runner page with "Run Validation" trigger
- [x] Rule: every requirement must be linked to at least one arch component
- [x] Rule: every requirement must be linked to at least one test case
- [x] Rule: naming convention check (IDs must follow REQ-XXXX / COMP-XXXX / TC-XXXX)
- [x] Validation result display: pass/fail per rule, list of violations with severity

## Phase 8: Quality Reports

- [x] Reports page with coverage metrics (req coverage %, test pass rate %)
- [x] Audit trail table (all create/update/delete/validate/export events with timestamp and user)
- [x] Exportable report view (HTML-formatted, print-friendly)
- [x] Coverage ring visualizations

## Phase 9: Timeline Module

- [x] Timeline nav item in sidebar
- [x] Chronological event list with type badges (milestone/change/note/todo/ai)
- [x] Manual entry form (title, content, type selector)
- [x] Todo checklist items within timeline entries
- [x] Filter by event type
- [x] Expand/collapse entries

## Phase 10: AI Assistant Panel

- [x] Floating/slide-in AI assistant panel (project-context-aware)
- [x] Mode selector: Draft Requirement / Draft Arch Note / Draft Test Case
- [x] LLM call with project context injected into system prompt
- [x] Markdown rendering via Streamdown

## Phase 11: Polish & Tests

- [x] Empty states for all list pages
- [x] Loading spinners for data-heavy pages
- [x] All 18 vitest tests passing (including new mocks for all new DB helpers)
- [x] Zero TypeScript errors
- [x] Final checkpoint
