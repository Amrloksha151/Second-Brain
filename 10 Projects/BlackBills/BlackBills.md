---
status: 📥 inbox
priority: medium
created: 2026-05-17
tags:
  - project
  - status/active
---
# BlackBills

## 🎯 Goal
An AI-integrated financial system and bill issuer designed for businesses of all scales and for developers. The primary focus is providing a robust, highly cost-efficient infrastructure for billing and financial management that undercuts traditional competitors.

## 🗺️ Milestones
- [ ] 1. Define Core Architecture and AI Integration Strategy.
- [ ] 2. Develop Merchant Onboarding and Bill Issuance Flow.
- [ ] 3. Implement Developer SDKs and Documentation.
- [ ] 4. Integrate Payment Gateways and Settlement Logic.
- [ ] 5. Beta testing with initial business partners.

## 🔗 Connections
- **Area:** [[Finance]]
- **Resources:** [[bill.com]], [[Wave]], [[Zoho Invoices]], [[Invoice Ninja]]
- **Inbox Reference:** [[2026-05-08]] thought regarding competitors.

## 📝 Notes
- **Competitive Edge:** 
	- Developer-first approach and scalability for all business sizes.
	- AI-driven automation for billing and reconciliation.
	- Significant cost efficiency compared to [[Wave]], [[Zoho Invoices]], and [[Invoice Ninja]].

- **Tech Stack:**
	- **Backend + API:** [[Django]] + [[Django Rest Framework]]
	- **Database:** [[PostgreSQL]] (Self-hosted)
	- **Frontend Web:** [[React]]
	- **Frontend Mobile:** [[React-Native]]
	- **Deployment:** [[Kubernetes]]
	- **API Docs:** [[AstroJS]] (with MD content collections)

- **Infrastructure & Budget:**
	- **Cloud Provider:** [[DigitalOcean]]
	- **Total Opening Budget:** $250 (Targeting ~$20/mo for Year 1)
	- **Monthly Breakdown:**
		- Managed Kubernetes (DOKS): $12/mo
		- Spaces Object Storage (250GB): $5/mo
		- Load Balancer: $15/mo (Planned for scaling phase)

- **Observability & Analytics:**
	- **User Analytics:** [[Google Analytics]]
	- **System Monitoring:** [[Grafana]] (system state/metrics)
	- **Logging & APM:** [[DataDog]] (logs and performance tracking)

- **Communications:**
	- **Email Delivery (Auth/Transactional):** [[Brevo]]
	- **Receiving Strategy:** 
		- **Phase 1:** Alias emails (early stage).
		- **Phase 2:** Custom [[SMTP]] servers (scaling phase).

- **Network & Server Architecture:**
	- **External Proxy:** [[Cloudflare Tunnels]] (Reverse Proxy)
	- **Internal Proxy & Static Handling:** [[Nginx]]
	- **Protocol Strategy:** 
		- Primary: [[HTTP/2]]
		- Restricted: [[HTTP/1.1]] (Limited to prevent request smuggling attacks)
