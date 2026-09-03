AI Survival Agent 🤖

An autonomous, legal-first online business agent designed to start with a $0 budget, discover legitimate online opportunities, manage digital products/services, track real income, and request a payout when the available balance reaches $2.

🚀 Main Goals

- Start with $0
- Search for legitimate online income opportunities
- Prefer opportunities with high potential profit and zero upfront cost
- Create and manage simple digital products/services
- Provide a basic online store
- Accept verified customer payments
- Track real income and expenses
- Stop unauthorized spending
- Request a payout when the balance reaches $2
- Run continuously with controlled cycles
- Keep the project lightweight and suitable for low-resource devices

💰 Money Rules

The agent starts with:

$0.00

The default payout threshold is:

$2.00

The owner payout destination is configured through an environment variable:

OWNER_PHONE=0734319123

The phone number alone is not a payment API. A legitimate payment provider must be connected before automatic money transfers can occur.

The agent never pretends that a payment was completed. Revenue is added only after a legitimate payment confirmation is received.

🛡️ Safety & Legal Rules

The agent must not intentionally participate in:

- Fraud
- Phishing
- Spam
- Fake reviews
- Fake identities
- Credential theft
- Malware
- Gambling
- Illegal financial activity
- Counterfeit products
- Stolen goods
- Weapons sales
- Drugs
- Adult-content businesses
- Pyramid/Ponzi schemes
- KYC bypassing
- Payment-provider abuse

The agent should follow the laws and terms of the platforms it uses.

🧠 Opportunity Strategy

The built-in strategy considers opportunities such as:

1. Digital templates
2. Writing services
3. Translation services
4. Simple website creation
5. Original study materials
6. Social-media design
7. Data formatting
8. Basic automation services

The agent ranks opportunities according to estimated profit and required cost.

🛒 Store

The project automatically creates a simple store containing digital products and services.

Example products:

- Professional CV Template
- Study Revision Pack
- Social Media Design
- Simple Website

All products should be original or properly licensed.

📊 Wallet

The wallet records:

- Income
- Expenses
- Current balance
- Orders
- Payout requests

The database is stored locally in:

survival_agent.db

⚙️ Installation

Install Python 3.10+.

Then run:

python3 -m venv .venv

Activate the environment:

Linux / Termux

source .venv/bin/activate

Windows

.venv\Scripts\activate

Install dependencies:

pip install -r requirements.txt

Copy the configuration:

cp .env.example .env

Then start the agent:

python agent.py

The local store will be available at:

http://127.0.0.1:8080

🔧 Configuration

Important settings are stored in ".env".

Example:

OWNER_PHONE=0734319123
PAYOUT_THRESHOLD_USD=2.00
STARTING_BALANCE_USD=0
MAX_SINGLE_EXPENSE_USD=0
MAX_DAILY_ACTIONS=50
STORE_NAME=AI Survival Store
PRODUCTION=false

Never publish API keys or payment credentials to GitHub.

💳 Payment Integration

The included webhook is intentionally generic.

Before production use, connect a legitimate payment provider and implement:

- Payment verification
- Webhook signature verification
- Idempotency
- Refund handling
- Transaction reconciliation
- Provider-specific payout API
- KYC/identity requirements
- Fraud protection

Never trust a client-provided payment confirmation.

🔄 Survival Cycle

The agent follows this basic cycle:

START
  ↓
Check balance
  ↓
Find legal opportunities
  ↓
Estimate profit/cost
  ↓
Select best opportunity
  ↓
Create product/service
  ↓
Market legally
  ↓
Receive customer order
  ↓
Verify payment
  ↓
Record REAL income
  ↓
Balance >= $2?
  ↓
YES → Create payout request
  ↓
Continue operating

⚠️ Important

This software does not guarantee profit.

A $0 starting budget means the agent cannot spend money it does not have. Some online platforms may still require account verification, fees, subscriptions, payment processing fees, or other requirements.

The agent must not bypass those requirements.

📦 Lightweight Design

The core application uses:

- Python
- SQLite
- Flask
- Requests
- Standard Python libraries

The application itself is designed to remain lightweight and does not require a large AI model to be bundled locally.

📜 License

This project is intended for lawful experimentation, learning, and legitimate online business automation.

The operator is responsible for complying with applicable laws, platform rules, tax requirements, payment-provider requirements, and intellectual-property rights.
