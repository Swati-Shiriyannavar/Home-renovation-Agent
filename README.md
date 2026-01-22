🏡✨ AI-Powered Home Renovation Planner (Multi-Agent System)


A production-style AI Home Renovation Planner Agent powered by Google ADK that:

Understands room photos, inspiration images, and text

Creates budget-aware renovation plans

Generates professional photorealistic renderings

Produces a complete renovation roadmap

Supports iterative design feedback

This project demonstrates how modern agentic AI systems are actually built—not toy demos.

✨ Key Features
🔍 Intelligent Image & Space Analysis

Upload room photos or inspiration images

Automatically detects layout, size, condition, and style

Identifies improvement opportunities

🎨 Photorealistic Design Generation

Creates high-quality renovation renderings using Gemini 3 Pro

Supports iterative visual edits (colors, lighting, flooring, fixtures)

💰 Budget-Aware Planning

Tailors recommendations based on budget constraints

Prioritizes high-impact upgrades

Provides realistic cost estimates

📊 End-to-End Renovation Roadmap

Budget breakdown

Timeline estimation

Contractor & material checklist

Step-by-step action plan

🤖 Real Multi-Agent Architecture

Coordinator / Dispatcher pattern

Sequential pipeline for complex workflows

Modular, extensible, and production-ready

🧠 System Architecture Overview

The system uses a Coordinator + Sequential Multi-Agent Pipeline:

Coordinator (Root Agent)
    ├── Info Agent (Quick Q&A)
    └── Renovation Planning Pipeline
          ├── Visual Assessor Agent
          ├── Design Planner Agent
          └── Project Coordinator Agent

Why This Architecture?

✅ Runs only the agents needed per request

✅ Clear separation of responsibilities

✅ Easy to extend (new tools, agents, workflows)

✅ Mirrors real-world agentic AI systems

🧩 Agent Responsibilities
📸 1. Visual Assessor Agent

Analyzes uploaded room photos

Extracts:

Layout & dimensions

Condition & constraints

Style cues from inspiration images

Identifies renovation opportunities

Provides rough cost estimates

🎨 2. Design Planner Agent

Creates a renovation design aligned with:

Budget

Style preferences

Space constraints

Specifies:

Materials

Colors

Fixtures

High-impact upgrades

🏗️ 3. Project Coordinator Agent

Generates:

Photorealistic renovation renderings

Budget breakdown

Project timeline

Action checklist

Handles iterative design updates and refinements

⚙️ Tech Stack & Capabilities

Google ADK – Multi-agent orchestration

Gemini 3 Flash – Fast reasoning & planning

Gemini 3 Pro – Multimodal image generation & refinement

Tool Calling:

google_search

estimate_renovation_cost

calculate_timeline

generate_renovation_rendering

edit_renovation_rendering

Versioned Artifacts – Automatic tracking of design iterations

🛠️ Step-by-Step Setup
1️⃣ Clone the Repository
git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
cd awesome-llm-apps/advanced_ai_agents/multi_agent_apps/ai_home_renovation_agent

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Configure Gemini API Key
export GOOGLE_API_KEY="your_gemini_api_key"


Or create a .env file:

GOOGLE_API_KEY=your_gemini_api_key

4️⃣ Launch the ADK Web Interface
cd multi_agent_apps
adk web

5️⃣ Open Your Browser

Select ai_home_renovation_agent from the ADK interface.

🧪 Example Use Cases
🟢 Scenario 1: Room Photo + Budget
[Upload kitchen photo]
"What can I improve here with a $5,000 budget?"


➡️ Space analysis → budget-friendly recommendations → rendering

🟢 Scenario 2: Room + Inspiration Image
[Upload your kitchen photo]
[Upload Pinterest inspiration]
"Make my kitchen look like this. What's the cost?"


➡️ Style extraction → tailored plan → rendering + budget

🟢 Scenario 3: Text-Only Planning
"Renovate my 10x12 kitchen.
Modern farmhouse style, white shaker cabinets.
Budget: $30k"


➡️ Design plan → rendering → full roadmap

🟢 Scenario 4: Iterative Refinement
"Make the cabinets cream instead of white"
"Add pendant lights over the island"
"Use lighter oak flooring"


➡️ Updated renderings with version history

✍️ Sample Prompts

“I want to renovate my small galley kitchen (8x12). Modern farmhouse style. Budget: $25k.”

“Turn my tiny bathroom (5x8) into a spa-like retreat with a walk-in shower. Budget: $15k.”

“Redesign my bedroom with an accent wall and new flooring. Budget: $12k.”
