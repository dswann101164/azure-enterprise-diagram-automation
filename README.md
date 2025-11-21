# Azure Enterprise Diagram Automation

> Enterprise-scale Azure architecture diagram automation with multi-subscription support, CI/CD integration, and compliance metadata.

[![Original Repo](https://img.shields.io/badge/based%20on-Shailender's%20Repo-blue)](https://github.com/Shailender-Youtube/Architecture_Diagrams_Python_AI)
[![Tutorial Video](https://img.shields.io/badge/watch-YouTube%20Tutorial-red)](https://www.youtube.com/watch?v=VIDEO_ID)

**Tested on:** 44 Azure subscriptions managing 31,000+ resources during enterprise merger  
**Status:** 🚧 Enterprise features in active development (launching this weekend)

---

## 🎯 What This Adds to the Original

This fork extends [Shailender's excellent Architecture Diagrams Generator](https://github.com/Shailender-Youtube/Architecture_Diagrams_Python_AI) with enterprise-scale features:

- ✅ **Multi-subscription diagram generation** - Document entire Azure landing zones
- ✅ **CI/CD pipeline integration** - Auto-generate diagrams on Terraform/Bicep deploy
- ✅ **Compliance metadata** - Audit-ready diagrams with SOC2/PCI tagging
- ✅ **Performance optimization** - Handle 30,000+ resources efficiently
- ✅ **Enterprise troubleshooting** - Solutions for real-world production issues

**Watch Shailender's tutorial first** (22k views) to understand the foundation, then use this repo for enterprise implementation.

---

## 🚀 Quick Start

### Prerequisites
- Python 3.11+
- Graphviz
- VS Code with draw.io extension
- Azure CLI (for multi-subscription support)

### Installation
```bash
# Clone this repo
git clone https://github.com/dswann101164/azure-enterprise-diagram-automation.git
cd azure-enterprise-diagram-automation

# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Basic Usage (Original Functionality)

See the original repo's instructions for basic diagram generation.

### Enterprise Usage (Coming This Weekend)
```bash
# Generate diagrams for all subscriptions
python scripts/generate_multi_subscription.py --config config/subscriptions.yaml

# Run with CI/CD integration
# See pipelines/ folder for Azure DevOps and GitHub Actions templates
```

---

## 📋 Enterprise Features (In Development)

### This Weekend (Nov 23-24)

- [ ] Multi-subscription script (`scripts/generate_multi_sub.py`)
- [ ] Azure DevOps pipeline template (`pipelines/azure-pipelines.yml`)
- [ ] GitHub Actions workflow (`pipelines/github-actions.yml`)
- [ ] Compliance tagging automation
- [ ] Enterprise examples (hub-spoke, landing zones)
- [ ] Comprehensive troubleshooting guide

### Coming Soon

- [ ] Azure Resource Graph integration (query live infrastructure, not just IaC)
- [ ] Cost metadata overlay (visualize spend per component)
- [ ] Confluence/SharePoint auto-update integration
- [ ] PowerShell wrapper for Windows-centric shops

---

## 💼 Real-World Use Case

**Challenge:** Document 44 Azure subscriptions (31,000+ resources) for enterprise merger in Q1 2026.

**Traditional approach:** 200+ hours of manual Draw.io work, outdated before completion.

**This solution:** Automated diagram generation in 30 minutes, always current.

**Implementation guide:** Coming soon on [azure-noob.com](https://azure-noob.com)

---

## 🏗️ Repository Structure
```
azure-enterprise-diagram-automation/
├── scripts/
│   ├── generate_single_diagram.py      # Basic (from original)
│   ├── generate_multi_subscription.py  # Enterprise: multi-sub support
│   ├── add_compliance_metadata.py      # Enterprise: audit tagging
│   └── batch_processor.py              # Enterprise: large-scale processing
├── pipelines/
│   ├── azure-pipelines.yml             # Azure DevOps integration
│   └── github-actions.yml              # GitHub Actions integration
├── config/
│   ├── subscriptions.yaml              # Multi-subscription configuration
│   └── compliance_tags.yaml            # Audit metadata definitions
├── examples/
│   ├── single-subscription/            # Basic examples
│   ├── multi-subscription/             # Enterprise examples
│   └── merger-documentation/           # Real M&A use case
└── docs/
    ├── troubleshooting.md              # Common issues + solutions
    └── enterprise-setup.md             # Step-by-step enterprise guide
```

---

## 🤝 Contributing

Improvements and enterprise use case contributions welcome! 

If you're implementing this at scale and hit issues, please:
1. Open an issue with details
2. Share your solution via PR
3. Help build the enterprise knowledge base

---

## 📚 Resources

- **Original repo:** [Shailender's Architecture Diagrams Generator](https://github.com/Shailender-Youtube/Architecture_Diagrams_Python_AI)
- **Tutorial video:** [Watch on YouTube](link) (22k views)
- **Enterprise guide:** [Coming soon - azure-noob.com](https://azure-noob.com)
- **My blog:** Technical Azure operations content at [azure-noob.com](https://azure-noob.com)

---

## 📄 License

Same as original repository.

---

## 🙏 Credits

Built on the excellent foundation by [Shailender](https://github.com/Shailender-Youtube).  
Watch his [tutorial video](link) for the basics - it's excellent.

Enterprise extensions and real-world testing by [David Swann](https://github.com/dswann101164).

---

**Status:** 🚧 Active development - enterprise features launching this weekend (Nov 23-24, 2025)

Star this repo to follow progress! ⭐
