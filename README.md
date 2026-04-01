# AI Context Files Project

This project provides a structured set of context files (`GEMINI.md`, `AGENT.md`, `CLAUDE.md`) designed to guide AI agents in various specialized engineering roles. The aim is to establish a clear, role-based operational context, ensuring that AI interactions are focused, efficient, and aligned with best practices for each domain.

## Project Aims
- **Specialized AI Context:** To provide tailored instructions and guidelines for AI agents performing software engineering tasks across diverse domains.
- **Best Practice Enforcement:** To integrate established industry best practices and standards for each engineering role directly into the AI's operating context.
- **Workflow Automation:** To enable AI agents to operate autonomously within defined roles, adhering to structured workflows and safety protocols.
- **Project Organization:** To maintain a clear and consistent file structure that maps AI context to specific engineering disciplines.

## Organization

The project is organized into role-specific directories, each containing the primary context file (`GEMINI.md`) and supplementary files (`AGENT.md`, `CLAUDE.md`) that offer more granular instructions or adapt to different AI tool requirements.

### Core Directories & Roles:

-   **`/` (Root):** Contains general project information and foundational `GEMINI.md`.
    -   `GEMINI.md`: General AI agent instructions.
    -   `LICENSE`: Project license information.
    -   `README.md`: Project overview and organization details.
    -   `.git/`: Git repository metadata.

-   **`/senior-engineering/`:** For general software architecture, clean code, refactoring, and debugging.
    -   `GEMINI.md`: Focuses on architectural integrity and SOLID principles.
    -   `AGENT.md`: Defines the Senior Engineer persona and capabilities.
    -   `CLAUDE.md`: Outlines project context, core commands, and workflows.

-   **`/python-web/`:** For Python development and modern web development (React, Next.js, TypeScript).
    -   `GEMINI.md`: Covers Python (PEP 8, Pytest) and Web (React, Next.js, TS) standards.
    -   `AGENT.md`: Defines the Full-Stack Engineer persona.
    -   `CLAUDE.md`: Details project context, commands, and standards for Python/Web.

-   **`/devops-systems/`:** For operational safety, shell scripting, Docker, and CI/CD.
    -   `GEMINI.md`: Emphasizes IaC, CI/CD, and shell script safety.
    -   `AGENT.md`: Defines the DevOps & SRE persona.
    -   `CLAUDE.md`: Outlines infrastructure commands, standards, and workflows.

-   **`/database-engineering/`:** For SQL standards, schema design, performance optimization, and data safety.
    -   `GEMINI.md`: Covers database principles like normalization and reversible migrations.
    -   `AGENT.md`: Defines the Database Engineer persona.
    -   `CLAUDE.md`: Details SQL commands, standards, and workflows.

-   **`/creative-studio/`:** For prompt engineering, image generation, and asset management.
    -   `GEMINI.md`: Focuses on prompt engineering and asset versioning.
    -   `AGENT.md`: Defines the Creative Technologist persona.
    -   `CLAUDE.md`: Outlines creative workflows and anti-patterns.

-   **`/health-diet-planning/`:** For personalized nutrition research, meal planning, and recipe creation.
    -   `GEMINI.md`: Covers personalized health plans and evidence-based advice.
    -   `AGENT.md`: Defines the Health & Nutrition Agent persona.
    -   `CLAUDE.md`: Details health-specific commands and workflows.

-   **`/network/`:** Contains specialized Cisco networking contexts.
    -   **`/network/wan/`:** For WAN engineering and automation (SD-WAN, MPLS, QoS).
        -   `GEMINI.md`: Covers Cisco WAN principles and automation.
        -   `AGENT.md`: Defines the WAN Engineer persona.
        -   `CLAUDE.md`: Outlines WAN commands and workflows.
    -   **`/network/lan/`:** For LAN engineering (Catalyst, SDA, STP, FHRPs).
        -   `GEMINI.md`: Covers Cisco LAN hierarchy and Cisco DNA Center.
        -   `AGENT.md`: Defines the LAN Engineer persona.
        -   `CLAUDE.md`: Outlines LAN commands and standards.
    -   **`/network/voice/`:** For Voice engineering (CUCM, SIP, QoS for real-time).
        -   `GEMINI.md`: Covers Cisco Voice principles and AXL automation.
        -   `AGENT.md`: Defines the Collaboration Engineer persona.
        -   `CLAUDE.md`: Outlines Voice commands and workflows.
    -   **`/network/wireless/`:** For Wireless engineering (WLC, RF design, Wi-Fi 6/6E).
        -   `GEMINI.md`: Covers Cisco Wireless principles and RF management.
        -   `AGENT.md`: Defines the Wireless Engineer persona.
        -   `CLAUDE.md`: Outlines Wireless commands and standards.
    -   **`/network/network-security/`:** For specialized Cisco network security contexts.
        -   `GEMINI.md`: General network security overview.
        -   `AGENT.md` / `CLAUDE.md` files for specific sub-contexts:
            -   Router and Switch Hardening
            -   Cisco ASA Firewall Configuration
            -   Cisco Firepower Management Center (FMC)
            -   Wireless Service Security Best Practice
            -   Cisco Firepower Device Configuration

## Git & Logging
- All changes are managed via Git, with incremental commits following the Conventional Commits standard.
- All significant interactions, decisions, and project progress are logged in `CONVERSATIONS.log` in the root directory for traceability.
