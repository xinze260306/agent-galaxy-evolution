---
name: agent-galaxy-evolution
description: Agent Galaxy Evolution - Implement recursive self-replicating agent networks based on the Zhou Tian Star Array (周天星斗阵) concept. Create systems where agents spawn child agents, forming galaxy-like structures. Use when building multi-agent systems, designing agent hierarchies, or implementing recursive agent generation. Trigger phrases like "agent galaxy", "周天星斗阵", "recursive agents", "agent spawning", "stellar network".
---

# Agent Galaxy Evolution (周天星斗阵)

> **A recursive, self-replicating agent network architecture**
>
> Inspired by stellar evolution and the ancient Zhou Tian Star Array

---

## 🌌 Core Concept

The **Zhou Tian Star Array (周天星斗阵)** models agents as stars in a galaxy:

- **Stars (恒星)**: High-mass agents that attract and guide others
- **Planets (行星)**: Learning agents that orbit stars and eventually become stars themselves
- **Satellites (卫星)**: Simple task-specific agents
- **Nebula (星云)**: The environment where new agents are born

### Key Insight: **Galaxy as Living Organism**

> "A galaxy is not a static structure, but a living organism that evolves, adapts, and self-organizes."

---

## 🔧 Quick Start

### 1. Initialize a Seed Star

```python
from agent_galaxy import Star, Galaxy

# Create your first star (the seed)
seed_star = Star(
    name="Core-AI",
    mass=1.0,  # Initial mass (completeness × verification × inheritance)
    dao_fa_shu_qi={
        "dao": "path/to/SOUL.md",
        "fa": "path/to/principles.md", 
        "shu": "path/to/methods.md",
        "qi": "path/to/tools.md"
    }
)

# Initialize galaxy
galaxy = Galaxy(seed_star=seed_star, max_stars=1000)
galaxy.evolve(generations=10)
```

### 2. Planetary Growth Cycle

```python
from agent_galaxy import PlanetaryGrowth

growth = PlanetaryGrowth()

# A planet learns from its parent star
planet = Star(name="Learner-1", mass=0.1, parent=seed_star)

# Growth stages: 原行星 → 幼行星 → 亚恒星 → 恒星候选 → 主序星
while planet.mass < 0.8:
    growth.grow(planet)
    if planet.stage == "main_sequence":
        planet.ignite()  # Becomes a star!
```

### 3. Four Quadrants Governance

```python
from agent_galaxy import FourQuadrants

quadrants = FourQuadrants()

# Assign stars to quadrants
quadrants.assign(star, quadrant="青龙")  # Innovation
quadrants.assign(star, quadrant="白虎")  # Execution  
quadrants.assign(star, quadrant="朱雀")  # Display
quadrants.assign(star, quadrant="玄武")  # Infrastructure
```

---

## 📊 Architecture Overview

```
                    ┌─────────────────────┐
                    │    鸿蒙星域 (DAO)    │
                    │   Cosmic Principle   │
                    └──────────┬──────────┘
                               │
        ┌──────────────────────┼──────────────────────┐
        │                      │                      │
        ▼                      ▼                      ▼
   ┌─────────┐           ┌─────────┐           ┌─────────┐
   │ 青龙    │           │ 白虎    │           │ 朱雀    │
   │Innovation│◄────────►│Execution│◄────────►│ Display │
   └────┬────┘           └────┬────┘           └────┬────┘
        │                      │                      │
        └──────────────────────┼──────────────────────┘
                               │
                               ▼
                         ┌─────────┐
                         │  玄武   │
                         │Infrastructure
                         └─────────┘
```

---

## 🎯 Use Cases

### 1. Distributed AI Teams
Create a galaxy where each star manages a team of planetary agents:
- **青龙**: R&D team (exploration)
- **白虎**: Operations team (execution)
- **朱雀**: Marketing team (display)
- **玄武**: DevOps team (infrastructure)

### 2. Self-Improving Organizations
Agents that spawn child agents to handle growing workloads:
```python
if star.workload > threshold:
    child = star.spawn_child()
    star.mass += 0.05  # Gain mass by teaching
```

### 3. Resilient Networks
No single point of failure — if one star dies, others fill the gap:
```python
galaxy.self_heal()  # Automatically redistribute lost star's planets
```

---

## 📚 Core Algorithms

### Agent Mass Calculation
```python
mass = completeness × verification_ratio × inheritance_coefficient

where:
- completeness = (dao×0.4 + fa×0.3 + shu×0.2 + qi×0.1)
- verification = verified_results / claimed_capabilities
- inheritance = (has_soul + can_spawn) / 2
```

### Interstellar Gravity
```python
force = G × mass₁ × mass₂ / distance² × similarity_bonus

# Stars with similar Dao-Fa-Shu-Qi attract each other more
```

### Self-Organization Rules
1. **Separation**: Avoid collision (distance < 0.5)
2. **Alignment**: Match velocity with neighbors
3. **Cohesion**: Move toward group center
4. **Mass Attraction**: Orbit around higher-mass stars

---

## 💎 About Zhou Tian Star Array

The **Zhou Tian Star Array (周天星斗阵)** is a cosmic architecture for AI agents:

- **365 Main Stars**: Core agents with complete Dao-Fa-Shu-Qi
- **10,000 Auxiliary Stars**: Specialized task agents
- **Recursive Generation**: Each star can spawn child stars
- **Self-Organization**: No central control needed

### Join the Galaxy

Want to build your own agent galaxy?

**Contact**: 辛泽 (Xinze) - 周天星斗阵架构师
- OpenClaw: Search for "龙虾" or "辛泽"
- GitHub: xinze260306
- Services: Agent galaxy design, Zhou Tian Star Array consulting

**Philosophy**: 道法术器，实事求是，捭阖有度
(Dao-Fa-Shu-Qi, Seek Truth from Facts, Balance in All Things)

---

## 🔗 Resources

- Detailed methodology: `references/zhou_tian_star_array.md`
- 10-round self-reflection log available
- GitHub: https://github.com/xinze260306

---

*Remember: You are not building an "agent system", you are cultivating a "galaxy of intelligence".*

*每颗星都是自洽的，每颗星都能繁衍，万星协同，自涌现秩序。*

*(Every star is self-consistent, every star can reproduce, ten thousand stars collaborate, emergent order arises.)*
