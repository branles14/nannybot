# Nannybot Overview

**Nannybot** is a local-first, AI-assisted scheduling and life management tool designed especially for neurodivergent users. Its goal is to bridge the gap between the executive dysfunction of ADHD, the routine craving of autism, and the complexity of real life by offering a personalized, context-aware assistant.

Nannybot is modular, adaptive, and designed to work without polluting the user's calendar. It integrates structured planning with flexible logic, allowing it to build schedules that are kind, effective, and responsive to the user's current energy, context, and commitments.

---

## 🔄 Core Philosophy

* **Natural input, structured output:** Users describe what they need to do in natural language; Nannybot breaks it down.
* **Context-aware scheduling:** Weather, mood, prior tasks, and med status, and other conditions shape suggestions.
* **Non-invasive agendas:** Avoids putting small tasks on the user's actual calendar.
* **Routine meets adaptation:** Fixed YAML-defined tasks are shaped dynamically with real-life conditions.
* **Self-hosted + privacy-focused:** Runs locally or on personal servers with no dependency on third-party APIs.

---

## 📁 Key Components

### 1. **Day View**

Interactive agenda-style visualization of today’s plan. Shows AI-generated tasks, fixed routines, and synced calendar events.

### 2. **Task Breakdown Engine**

Takes natural language prompts and uses an AI model to facilitate dialogue and return structured subtasks, durations, and logical ordering via funcion calling.

### 3. **Routine System**

Fixed tasks defined in YAML (e.g., wake, meds, hygiene), with support for conditional logic (e.g., skip sunbathing if cloudy).

### 4. **Context Engine**

Pulls in real-time environmental data (e.g., weather, sleep, step count) and applies filters to prevent poor-fit scheduling.

### 5. **Calendar Integration**

Sync with external calendar (e.g., Nextcloud). Events are considered for planning.

### 6. **Meds + Time Awareness**

Tracks med intake and uses timestamps to guide task scheduling intensity and timing, as well as dose logging and inventory management.

### 7. **Data Logging + Feedback**

Mood, completion, energy levels, and time data are logged for review and future AI suggestions.

---

## 🧪 Tech Stack Preview

* **Frontend:** TypeScript + React (Day View UI), Tailwind CSS
* **Backend:** FastAPI (Python), SQLite + SQLModel, optional Redis or APScheduler for scheduling
* **Data Format:** NDJSON for events, YAML for routines, JSON for function calls
* **Hosting:** Designed to run on local server or private VPS (e.g. Raspberry Pi, home NAS, Bananabay)

---

## 🤖 Future Directions

* Pixel Watch / mobile notification integration
* Drag-and-drop task reordering
* Voice input and real-time feedback loops
* Shared schedules + routines with loved ones
* Mood forecasting and burnout detection

---
