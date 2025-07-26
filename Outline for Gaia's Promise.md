# Create folder structure and markdown content for Obsidian vault
base_path = Path("/mnt/data/Gaias_Promise_Vault")
pages = {
    "00 - Project Gaia's Promise Hub.md": """# 🌱 Project Gaia's Promise
*A Sacred-Scientific Initiative for the Renewal of the Garou Nation*

## Overview
Blending cutting-edge genetics, spirit work, ancient Apis rites, and Garou traditions to heal the bloodlines and increase birth rates across Gaia’s children.

---

## 🔗 Quick Links
- [[01 - Scientific Branch (Noc)]]
- [[02 - Spiritual Branch (Karma)]]
- [[03 - Joint Initiatives]]
- [[04 - Sanctum Vitae]]
- [[05 - The Emerald Accord]]
- [[06 - Soul + Cell Symposium]]
- [[07 - Honoring Riegel]]
""",

    "01 - Scientific Branch (Noc).md": """# 🧬 Scientific Branch (Led by Noc Rhaegis)

## Mission
To research and apply advanced genetics and Glasswalker tech in service to Garou fertility, hybrid viability, and genetic harmony with Gaia.

### 🧪 Focus Areas
- **Genetic Recovery Archives (Riegel’s Legacy)**
- **Hybrid Viability Studies**
- **The Curse Suppression Serum ("Mercy Gene")**
- **Conception Tracking & Viability Algorithms**

See [[03 - Joint Initiatives]] for collaborative efforts.
""",

    "02 - Spiritual Branch (Karma).md": """# 🐝 Spiritual Branch (Led by Karma Orks)

## Mission
To reawaken sacred rites, empower conception with spirit allies, and honor the ancient Apis role as Gaia’s Wombkeepers.

### ✨ Focus Areas
- **Apis Rites of Quickening**
- **Temple Womb Sanctuaries**
- **Calling the Unborn**
- **Ritual of Three Threads**

See [[03 - Joint Initiatives]] for shared endeavors with Noc.
""",

    "03 - Joint Initiatives.md": """# 🤝 Joint Initiatives

## 🔗 Collaborations Between Noc & Karma

### **Sanctum Vitae (The Living Archive)**
- Hybrid library of spirit-bound lore, genetic logs, family shrines, and lost-line remembrance.

### **The Emerald Accord**
- Quarterly ethics and oversight council with members from every shifter lineage.

### **Soul + Cell Symposium**
- Annual celebration of science, ritual, and storytelling to share breakthroughs and renew the cause.

Includes projects from:
- [[01 - Scientific Branch (Noc)]]
- [[02 - Spiritual Branch (Karma)]]
""",

    "04 - Sanctum Vitae.md": """# 🏛️ Sanctum Vitae

## Overview
A dual-nature structure both in the Umbra and physical world. Home to:
- Riegel’s journals and spirit-bound teachings
- Genetic & spiritual records of Project Gaia’s Promise
- Family trees and ancestral shrines

Includes central altar in Riegel’s memory. See [[07 - Honoring Riegel]].
""",

    "05 - The Emerald Accord.md": """# 🟢 The Emerald Accord

## Purpose
An oversight body ensuring sacred and scientific fertility interventions remain ethical, consensual, and in alignment with Gaia's will.

## Members
- Garou (all tribes)
- Kinfolk
- Bastet, Corax, and other Fera reps
- Spirit emissaries

Meets quarterly in person or in dreamspace.
""",

    "06 - Soul + Cell Symposium.md": """# 🧠✨ Soul + Cell Symposium

## Description
An annual event where scientists, ritualists, shamanic practitioners, and spiritual midwives share findings, give workshops, and perform rites.

Each presentation given equal reverence—labs, rituals, and storytelling are all honored.

Hosted at:
- [[Sanctum Vitae]]
- Umbra reflections accessible by accorded invitation
""",

    "07 - Honoring Riegel.md": """# 🕯️ Honoring Riegel Orks

## Memorial Elements
- Lock of hair sealed in silver and wax
- Mobius strip sculpture from Umbral stone
- Holographic interface: AI personality advisor named "Riegel"

## Legacy Projects
- Genetic Archives
- Curse research foundations
- Spirit-tech communication protocols

Riegel’s influence continues through Karma, Noc, and every cub born by his foresight.
"""
}

# Create directory and write files
base_path.mkdir(parents=True, exist_ok=True)
for filename, content in pages.items():
    (base_path / filename).write_text(content)

# Return path for download
base_path

