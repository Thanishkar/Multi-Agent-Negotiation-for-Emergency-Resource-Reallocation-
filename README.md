
# 🏥 NEXUS
### Real-Time Multi-Agent AI Coordination for Hospital Emergencies

> **We built the AI brain that runs underneath the hospital—so clinicians can focus entirely on the patient in front of them.**

---

## 🚨 The Problem

Every day, hospitals face critical emergencies where life-saving resources are limited.

Doctors must decide, within seconds:

- Which patient gets the last ICU bed
- Which operating theatre should be used first
- Which surgeon should respond
- How ventilators and medical equipment should be allocated

These decisions are often made under immense pressure with fragmented information.

Patients don't always lose their lives because resources are unavailable—they lose them because coordinating those resources in real time is incredibly difficult.

---

## 💡 Our Solution

**NEXUS** is a **real-time multi-agent AI coordination platform** that intelligently allocates hospital resources during emergencies.

Instead of relying on a single AI model, every critical hospital resource is represented by its own specialized AI agent.

Examples include:

- 🛏 ICU Agent
- 🏥 Operating Theatre Agent
- 👨‍⚕️ Staff Agent
- 🫁 Equipment Agent
- 🎯 Orchestrator Agent

Each agent has its own goals, constraints, and responsibilities.

When an emergency occurs, the agents negotiate with one another and collaboratively produce an optimized allocation plan in **under 15 seconds**.

Every recommendation is accompanied by a clear, human-readable explanation.

---

# ✨ Key Features

## 🤝 Live Multi-Agent Negotiation

Watch AI agents coordinate in real time.

Example:

- ICU Agent releases Bed 3
- OT Agent postpones a non-critical surgery
- Staff Agent assigns the on-call surgeon
- Equipment Agent reallocates a ventilator

The negotiation is streamed live like a hospital command center.

---

## 🔍 Explainable Decision Making

Every allocation includes plain-English reasoning.

Example:

> "Patient 7 receives ICU Bed 2 because their predicted survival gain is highest while maintaining ventilator availability for incoming trauma cases."

No black-box decisions.

---

## 🔄 Counterfactual Decision Engine

After generating the allocation plan, NEXUS evaluates alternative scenarios.

Example:

> If Surgeon A had been assigned to Patient 2 instead of Patient 5, Patient 5's survival probability would decrease from **81%** to **58%**.

This enables doctors to understand **why** the recommended decision was chosen.

---

## 👨‍⚕️ Human-in-the-Loop Override

Doctors always remain in control.

If a clinician overrides any recommendation:

- The system instantly recalculates downstream allocations.
- Every affected resource is updated automatically.
- Ripple effects are visualized in real time.

AI assists.
Humans decide.

---

# 🏗 Architecture

```
               +----------------+
               |  Orchestrator  |
               +--------+-------+
                        |
     -----------------------------------------
     |        |         |         |           |
+---------+ +------+ +-------+ +---------+ +-----------+
| ICU AI  | | OT AI| |Staff AI| |Equip AI| |Future AI...|
+---------+ +------+ +-------+ +---------+ +-----------+
        \        |         |         /
         \       |         |        /
          -------- Shared State -------
                 (JSON Resource Model)
                        |
                 FastAPI + WebSockets
                        |
                  React Dashboard UI
```

### Backend

- FastAPI
- WebSockets
- Python

### Frontend

- React
- Live negotiation dashboard
- Resource allocation grid

### AI Layer

- Multi-Agent LLM architecture
- Role-specific reasoning agents
- Shared resource state
- Explainable decision generation

---

# ⚙ Workflow

1. Emergency event is received.
2. Resource state is loaded.
3. AI agents negotiate simultaneously.
4. Optimized allocation plan is generated.
5. Decisions are explained in plain English.
6. Counterfactual scenarios are evaluated.
7. Doctors may override any recommendation.
8. Ripple analysis updates the entire plan instantly.

---

# 🎬 Demo Scenario

### Highway Mass Casualty Incident

**Incoming**

- 🚑 9 Critical Patients

**Available Resources**

- 🛏 2 ICU Beds
- 🏥 1 Operating Theatre
- 👨‍⚕️ 4 Surgeons
- 🫁 3 Ventilators

### What Happens

✅ Agents negotiate live (~11 seconds)

✅ Complete allocation plan is generated

✅ Every decision is explained

✅ Counterfactual analysis is displayed

✅ Manual override instantly recalculates downstream effects

---

# 🌟 What Makes NEXUS Different?

- 🧠 Multi-Agent AI instead of a single chatbot
- ⚡ Real-time negotiation between hospital resources
- 📖 Fully explainable recommendations
- 🔍 Counterfactual reasoning for every decision
- 👨‍⚕️ Human-in-the-loop control
- 🔄 Instant ripple analysis after manual overrides
- 📡 Live streaming coordination dashboard

---

# 🚀 Vision

Healthcare professionals should never have to choose between speed and confidence during emergencies.

NEXUS transforms fragmented hospital resource management into a transparent, explainable, and collaborative AI-driven decision system—helping hospitals respond faster, smarter, and with greater trust.

> **AI coordinates the system. Doctors save the lives.**
