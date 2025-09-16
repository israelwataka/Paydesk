# PayDesk

**PayDesk** is a multi-tenant payment confirmation dashboard for businesses.  
It centralizes **M-Pesa** and **Airtel Money** transactions into one secure platform,  
allowing staff to confirm payments without exposing account balances.  

---

## 🚀 Features
- 🌐 **Multi-Tenant Support** → Each business gets its own subdomain (`yourbiz.paydesk.com`).
- 👥 **Role-Based Access** → Admin, Manager, and Attendant roles with different privileges.
- 💳 **Mobile Money Integrations** → Real-time webhooks from **M-Pesa Daraja** and **Airtel Money APIs**.
- 🔎 **Transaction Filtering** → Search payments by phone, date, amount, or reference.
- ✅ **Confirmation Workflow** → Staff confirm/reject transactions, with full audit trails.
- 🔒 **Privacy First** → Account balances are masked/hidden from attendants.
- 📊 **Reports & Exports** → Generate reports and summaries for business insights.
- 🛡️ **Super Admin Dashboard** → Manage tenants, billing, and system monitoring.

---

## 🏗️ Tech Stack
- **Backend**: Node.js (Express/NestJS) or PHP (Laravel)  
- **Frontend**: React / Next.js  
- **Database**: PostgreSQL / MySQL with tenant isolation  
- **Auth**: JWT or session-based with RBAC  
- **Hosting**: Supports wildcard SSL & subdomains (`*.paydesk.com`)  

---

## 📦 Installation (Development Setup)

```bash
# Clone repo
git clone https://github.com/yourusername/paydesk.git

# Install dependencies
cd paydesk
npm install   # or composer install (if using Laravel)

# Configure environment variables
cp .env.example .env
# Add DB credentials, Daraja & Airtel API keys, and base domain

# Run development server
npm run dev   # or php artisan serve
