<div align="center">Pedro
Network & Infrastructure Engineering | Systems Administration | Cloud | Automation | Software Development
I design, administer, troubleshoot, and improve infrastructure — from switches, domain controllers, and firewalls to cloud services, databases, and applications.


</div>About me
I'm a technology professional with a strong focus on network administration, infrastructure engineering, Windows and Linux systems, security, cloud operations, and automation. I work with the details that keep services available: IP addressing, VLANs, directory services, authentication, DNS, DHCP, firewall rules, routing, certificates, servers, virtualization, backups, and application dependencies.

My work spans both day-to-day operations and engineering. I investigate incidents using logs, packet traces, service status, configuration comparisons, and controlled tests. When a recurring problem needs more than a manual fix, I develop scripts, APIs, utilities, and internal software to improve reliability and reduce operational effort.

I also study artificial intelligence from its technical foundations and model behavior to practical integration and end-user experience. I use Hermes as one of several experimental environments to evaluate agents, tool use, reliability, limitations, and verification. AI is an area I test and understand—not a substitute for systems knowledge, engineering judgment, or independent validation.
My approach: Understand the environment → Gather evidence → Isolate the cause → Plan a safe change → Validate → Document.

Areas of expertise and practical experience
Domain	Technologies, activities, and engineering concerns
Network administration	TCP/IP, IPv4 addressing and subnetting, VLANs, managed switches, access and uplink ports, routing, DHCP, DNS, NAT, PPPoE, multi-WAN, network troubleshooting
Network security	pfSense, firewall policy, aliases and rule evaluation, VPNs (including OpenVPN), traffic analysis, pfBlockerNG, segmentation, PacketFence/NAC exploration
Identity & directory services	Windows Server, Active Directory, Samba AD DC (including Samba 4), domain-joined computers, DNS dependencies, authentication, user/group administration, access controls, domain troubleshooting
Linux & Windows operations	Ubuntu Server, Linux services, systemd, Windows 11/Server, PowerShell, Bash, WSL2, logs, permissions, service recovery, troubleshooting
Virtualization & containers	Proxmox VE, virtual machines, Docker, containerized services, service health, backup and restore considerations
Cloud engineering	AWS and Oracle Cloud Infrastructure (OCI), command-line diagnosis, networking/service dependencies, load balancing, TLS, cloud-hosted services, Terraform infrastructure definitions for database provisioning and configuration
Databases & backends	PostgreSQL, SQL, database backups and restoration, schemas and migrations, SQLAlchemy, Alembic, FastAPI, REST APIs
Software & scripting	Python, PowerShell, Bash, C++, C#, .NET, TypeScript, API integration, diagnostic and reporting tools
Delivery & observability	Git, GitHub, GitHub Actions, CI/CD, automated checks, regression tests, structured logs, JSON/CSV reports, technical runbooks
Hardware & integration	Device connectivity, Arduino Leonardo, C++, USB HID, hardware and network troubleshooting


Engineering in practice
The following are examples of the kinds of environments and problems I work on. They describe technical scope and methods, not a claim that every referenced environment or project is publicly available.
Network infrastructure, routing & security
My network work combines configuration with evidence-driven troubleshooting. I investigate how traffic actually moves through switches, VLAN interfaces, gateways, firewall policies, VPN tunnels, and external links—rather than relying solely on what the configuration appears to say.
- pfSense administration: WAN/LAN interfaces, VLAN interfaces, DHCP and DNS services, NAT behavior, firewall policies, packet filtering, aliases, and rule troubleshooting.
- Segmentation and switching: access ports versus uplinks, VLAN membership, unexpected DHCP leases, incorrect subnets, gateway reachability, and Layer 2/Layer 3 boundaries.
- Internet connectivity: PPPoE, bridge-mode modem integration, multi-WAN considerations, default gateways, upstream failures, and path verification.
- VPNs: OpenVPN client configuration, certificate compatibility, routes, tunnel reachability, and secure remote access troubleshooting.
- Traffic investigation: tcpdump, PCAP inspection, DNS lookups, ping, traceroute, socket tests, and firewall log correlation to understand dropped or misrouted traffic.
- Network security tooling: pfBlockerNG DNSBL behavior and whitelist troubleshooting; evaluation of NAC and PacketFence concepts.
Typical diagnostic question: Is the fault caused by switching, address assignment, DNS resolution, routing, a security policy, a certificate, or the application itself?
Identity, Windows Server & Samba Active Directory
I work with Windows and Linux environments where identity and name resolution are core infrastructure services. This includes Microsoft Active Directory and Samba 4 acting as an Active Directory Domain Controller (AD DC).
- Domain infrastructure and the interaction between DNS, authentication, client connectivity, and directory services.
- User and group administration, permissions, access requirements, and the operational impact of directory changes.
- Diagnosing domain-join and authentication failures, connectivity to domain services, and Windows client behavior.
- Windows system and application troubleshooting with PowerShell, native service tools, logs, and command-line diagnostics.
- Samba-based domain environments, Linux/Windows interoperability, and configuration or recovery investigations.
I treat directory services as critical infrastructure: changes require awareness of authentication dependencies, administrative access, and recovery options.
Cloud platforms, Terraform & database infrastructure
My cloud experience covers AWS and Oracle Cloud Infrastructure (OCI), with attention to operational troubleshooting as well as infrastructure configuration.

AWS
- Use of AWS CLI to inspect cloud resources and compare configuration with actual service behavior.
- Analysis of Application Load Balancers, DNS endpoints, HTTPS connectivity, and TLS certificate behavior.
- Verification of certificate trust chains, hostname matching, and SNI using tools such as OpenSSL.
- Investigation of application availability and infrastructure dependencies when a cloud-hosted service produces connection or security errors.
- Understanding the relationship between compute, network paths, load balancers, certificates, and application health.
Oracle Cloud Infrastructure & Infrastructure as Code
- Practical exposure to OCI-hosted infrastructure and its configuration and administration.
- Terraform definitions for database infrastructure, including provisioning and configuration workflows.
- Working with declarative infrastructure concepts, configuration parameters, resource dependencies, and validation before applying changes.
- Attention to credentials, configuration consistency, controlled changes, and avoiding secrets in version control.
I distinguish infrastructure that has been configured, tested, or investigated from services that are continuously operated in production; a public README should not imply certifications or operational scale that cannot be substantiated.
Email infrastructure & service delivery
Email reliability requires looking beyond an application-level “send” action. My troubleshooting covers the full delivery path, including:
- Postfix, SMTP sessions, submission ports, server responses, STARTTLS and TLS negotiation.
- Proxmox Mail Gateway (PMG), mail queue inspection, retry behavior, and transport troubleshooting.
- Zextras mail environments, message queues, delivery status, and operational command-line checks.
- Diagnosing whether failures originate in the application, authentication, transport encryption, gateway, mail queue, or destination service.
- Using logs and protocol-level tests to verify connectivity and delivery behavior.
Virtualization, recovery & operational continuity
- Linux services and Windows hosts in physical, virtualized, and containerized environments.
- Proxmox VE and Docker as part of infrastructure operations and application deployment.
- Creating inventories of configurations and service dependencies to support troubleshooting or recovery.
- Backups with integrity verification, including checksums and database dump validation.
- Restore planning, retention considerations, and explicit separation of backups from proof of recoverability.
- Investigating disk images, lost files, configuration artifacts, and recovery limits without claiming success when evidence is incomplete.
Software engineering & systems development
I develop software both as an engineering discipline and as a way to solve real operational problems. My focus includes API design, reliable data flows, diagnostics, safe migrations, tests, reporting, and maintainability.
Sindy — condominium & service management
Work on a web application for administrative and operational processes in condominium and service management. The engineering work includes:
- FastAPI, PostgreSQL, SQLAlchemy, and Alembic.
- API and database evolution, schema migrations, dependency and integrity checks.
- Deployment workflows, application health checks, and environment troubleshooting.
- Backup artifact inspection, checksums, database dump validation, and recovery-oriented documentation.
- Git branches, code review, CI checks, and careful separation between development changes and production operations.
Emphasis: Data integrity · safe migrations · application reliability · documented changes.
RECAELJ — business administration & operations
Iterative development and improvement of business software covering:
- Service orders, workshop operations, budgets, and customer-facing documents.
- Inventory and separation of items for resale versus workshop use.
- Financial processes, cash flow, banking views, manual entries, and reporting.
- Responsive interfaces, navigation, practical workflows, and usability improvements.
- Release-to-release checks, regressions, and controlled feature adjustments.
- Requirements and integration investigation for Brazilian electronic service invoicing.
Emphasis: Translating operational needs into software · functional validation · gradual improvement.

<sub>These applications involve private or operational work. Descriptions are intentionally limited to non-sensitive engineering information; they are not links to publicly available source code.</sub>
AI systems — understanding, evaluation & experimentation
I study AI across the stack: how models behave, what their limitations are, how tools and context affect outputs, and what the end user actually experiences. My interest is in understanding the technology and assessing where it is useful, reliable, or unsuitable.

The Hermes environment is one of my practical testbeds for this work:
- Comparing manual and agent-assisted technical workflows, including where automation introduces new risks.
- Examining tool invocation, reusable skills, context retrieval, knowledge indexing, and structured handoffs.
- Studying model outputs, factual grounding, error patterns, verification, and recovery after unsuccessful actions.
- Organizing technical knowledge so experiments can be repeated and conclusions reviewed.
- Using local research data, validation rules, and sanitized test fixtures to separate evidence from assumptions.
- Evaluating interfaces and workflows from the perspective of both the systems operator and the end user.
I do not equate a convincing AI answer with a verified technical result. Logs, source code, tests, and observed system behavior remain the basis for engineering decisions.
Public engineering projects
These repositories showcase network tools, monitoring, automation, APIs, data-oriented software, and hardware experiments. Project scope is described at a high level; each repository is the source of truth for its current functionality and limitations.
Networking, security & diagnostics
Repository	Engineering purpose	Main stack
NetForge IaC	Validate VLAN, subnet, gateway, and DHCP inventory; assist configuration and documentation generation.	Python
PacketLens	Offline analysis of classic PCAP captures, summarizing traffic and protocol indicators.	C++ · CMake
Lantern	Concurrent TCP service inventory for private IPv4 networks with structured output.	C++
Subnet Manager API	API for networks, VLANs, reservations, and address-conflict validation.	C# · ASP.NET Core
Topology Mapper	Produce Mermaid, Graphviz, and JSON network representations from structured information.	C# · .NET
WiFi Audit Report	Turn wireless survey CSV data into diagnostic HTML/JSON reports.	Python


Monitoring, operations & recovery
Repository	Engineering purpose	Main stack
InfraPulse	HTTP, API, and TCP availability checks with machine-readable metrics.	C# · .NET 8
Windows Network Watcher	Watch gateway, internet, and DNS connectivity; record structured incidents.	C# · .NET 8
Homelab Backup Manager	Compressed configuration backups, SHA-256 verification, and retention/restore workflows.	Python


Software, AI evaluation & hardware
Repository	Engineering purpose	Main stack
Claim Verifier	Distinguish supported evidence from inference and unverified claims.	Python
Remédio Aberto	Local-first exploration of official Brazilian medication information.	TypeScript
Leonardo DeskPad	USB HID macro-pad experiment with physical controls and input handling.	Arduino · C++
Arduino Network Control Panel	Explore the interface between hardware controls and network/software behavior.	Arduino


Explore all public repositories
How I investigate and deliver changes
                  INCIDENT / REQUIREMENT
                           |
                  Understand the context
                           |
                Collect objective evidence
                           |
               Isolate cause or constraints
                           |
                 Evaluate risk and rollback
                           |
                 Implement controlled change
                           |
            Verify result and check regressions
                           |
                 Document and monitor
My priorities are least privilege, reproducible tests, clear technical evidence, sensible backups, rollback planning, useful observability, and documentation that another administrator can follow. I prefer reliable changes over impressive-looking but unverified claims.
Technical toolkit at a glance
pfSense · TCP/IP · VLANs · Routing · VPN · DNS · DHCP · Active Directory · Samba AD DC · Windows Server · Ubuntu Server · Linux · Proxmox · Docker · AWS · Oracle Cloud · Terraform · PostgreSQL · FastAPI · Python · PowerShell · Bash · C++ · C# · .NET · TypeScript · GitHub Actions · SMTP · Postfix · PMG · Zextras
GitHub activity
<div align="center"><img src="https://github-readme-stats.vercel.app/api?username=pedvrezz&show_icons=true&hide_border=true&theme=transparent" height="155" alt="GitHub repository activity statistics" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=pedvrezz&layout=compact&langs_count=8&hide_border=true&theme=transparent" height="155" alt="Languages in public repositories" /></div><sub>These third-party widgets depend on external services and may occasionally be unavailable. Language distribution is based on repository metadata, not a proficiency score.</sub>
<div align="center">Reliable networks. Maintainable systems. Evidence-based engineering.

GitHub profile · Public repositories
</div>
