# GlimmerAdmin 💎

The professional administrative dashboard for the **Glimmer** e-commerce ecosystem. This project provides a powerful interface to manage products, categories, orders, and analytics for the GlimmerStore.

> [!IMPORTANT]
> This is the **Admin Panel** part of the project. To see the customer-facing storefront, visit [GlimmerStore](https://github.com/ibragmv/GlimmerStore).


## 🏗 Project Architecture
Glimmer is built as a decoupled full-stack application:
1. **GlimmerAdmin** (This repo): Dashboard for management and inventory control.
2. **[GlimmerStore](https://github.com/ibragmv/GlimmerStore)**: The customer-facing storefront.

## ✨ Admin Features
- **Dashboard Overview:** Real-time statistics on sales, revenue, and active users.
- **Inventory Management:** Full CRUD (Create, Read, Update, Delete) functionality for products and variants.
- **Order Tracking:** Monitor order statuses, payments, and shipping updates.
- **Content Management:** Manage categories, banners, and promotional content.
- **Analytics:** Visual data representation using modern charting libraries.

## 🛠 Tech Stack
- **Runtime:** [Bun](https://bun.sh/)
- **Frontend Framework:** React / Next.js (Change if you use Vue/Svelte)
- **Styling:** Tailwind CSS
- **State Management:** Zustand / TanStack Query
- **Tooling:** Vite / TypeScript

## 🚀 Installation & Setup

Ensure you have [Bun](https://bun.sh/) installed.

### 1. Clone the repo
```bash
git clone https://github.com/ibragmv/GlimmerAdmin.git
cd GlimmerAdmin
```

### 2. Install dependencies
```bash
bun install
```

### 3. Environment Variables
Rename a `.env.local` file and add your backend/API keys:
```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="clerk_public_key"
CLERK_SECRET_KEY="clerk_secret_key"

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

DATABASE_URL='database_url'

NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME="your_cloudinary_name"

FRONTEND_STORE_URL="store_url" # in developer mode - http://localhost:3001

STRIPE_API_KEY="secret_stripe_key"
STRIPE_WEBHOOK_SECRET="your_stripe_webhook_key"
```

### 4. Run development server
```bash
bun run dev
```

## 🤝 Relationship with GlimmerStore
This admin panel interacts with the same database/API as the **GlimmerStore**. Any changes made here (adding a product, updating a price) will reflect instantly on the storefront.

## 📄 License
This project is licensed under the MIT License.

---
