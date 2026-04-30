# SmartFin

SmartFin is a modern banking platform for everyone. Built with Next.js, SmartFin is a financial SaaS platform that connects to multiple bank accounts, displays transactions in real-time, allows users to transfer money to other platform users, and manages their finances altogether.

## ⚙️ Tech Stack

- **Framework:** [Next.js](https://nextjs.org/)
- **Language:** [TypeScript](https://www.typescriptlang.org/)
- **Backend as a Service:** [Appwrite](https://appwrite.io/)
- **Banking API:** [Plaid](https://plaid.com/)
- **Payments & Transfers:** [Dwolla](https://www.dwolla.com/)
- **Styling:** [TailwindCSS](https://tailwindcss.com/) & [Shadcn UI](https://ui.shadcn.com/)
- **Forms & Validation:** [React Hook Form](https://react-hook-form.com/) & [Zod](https://zod.dev/)
- **Charts:** [Chart.js](https://www.chartjs.org/)

## 🔋 Features

👉 **Authentication:** Ultra-secure SSR authentication with proper validations and authorization.  
👉 **Connect Banks:** Integrates with Plaid for multiple bank account linking.  
👉 **Dashboard:** Shows a general overview of user accounts with total balances from all connected banks, recent transactions, and money spent on different categories.  
👉 **My Banks:** Check the complete list of all connected banks with respective balances and account details.  
👉 **Transaction History:** Includes pagination and filtering options for viewing the transaction history of different banks.  
👉 **Funds Transfer:** Allows users to transfer funds using Dwolla to other accounts with required fields and recipient bank IDs.  
👉 **Real-time Updates:** Reflects changes across all relevant pages seamlessly.  
👉 **Fully Responsive:** Ensures the application adapts seamlessly to various screen sizes and devices, providing a consistent user experience across desktop, tablet, and mobile platforms.

## 🤸 Quick Start

Follow these steps to set up the project locally on your machine.

### Prerequisites

Make sure you have the following installed on your machine:
- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

### Installation

1. Clone the repository
```bash
git clone https://github.com/your-username/SmartFin.git
cd SmartFin/SmartFin
```

2. Install the project dependencies using npm:
```bash
npm install
```

3. Set Up Environment Variables
Create a new file named `.env` in the root of your project (`SmartFin/SmartFin/.env`) and add the following content:

```env
#NEXT
NEXT_PUBLIC_SITE_URL=http://localhost:3000

#APPWRITE
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
APPWRITE_DATABASE_ID=
APPWRITE_USER_COLLECTION_ID=
APPWRITE_ITEM_COLLECTION_ID=
APPWRITE_BANK_COLLECTION_ID=
APPWRITE_TRANSACTION_COLLECTION_ID=
NEXT_APPWRITE_KEY=

#PLAID
PLAID_CLIENT_ID=
PLAID_SECRET=
PLAID_ENV=sandbox
PLAID_PRODUCTS=auth,transactions,identity
PLAID_COUNTRY_CODES=US,CA

#DWOLLA
DWOLLA_KEY=
DWOLLA_SECRET=
DWOLLA_BASE_URL=https://api-sandbox.dwolla.com
DWOLLA_ENV=sandbox
```
*Note: Replace the placeholder values with your actual API credentials from Appwrite, Plaid, and Dwolla.*

4. Running the Project
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser to view the project.
