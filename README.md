# learnza-e-library

An open-source digital e-library web application engineered for high-performance reading experiences. Powered by Supabase for relational data storage and user authentication, Netlify for edge-optimized static hosting, and custom Cloudflare Workers for edge-based cross-origin document downloads.

## Architecture and Stack

* **Frontend**: Vanilla ES6+ JavaScript, Semantic HTML5, Modular CSS3
* **Backend as a Service**: Supabase (PostgreSQL, Row-Level Security, GoTrue Auth)
* **Edge Infrastructure**: Cloudflare Workers (CORS streaming proxy)
* **Hosting**: Netlify CI/CD

## Key Features

* **Relational Book Catalog**: Real-time filtering, category sorting, search indexing, and pagination backed by Supabase.
* **Edge Download Engine**: Custom Cloudflare Worker bypasses browser CORS limits and enforces direct attachment streaming for PDF resources.
* **Authentication and Roles**: Role-based access control (RBAC) separating student readers from catalog administrators.
* **Zero Heavy Frameworks**: Pure vanilla web performance yielding sub-second First Contentful Paint (FCP).

## Getting Started

### Prerequisites
* Modern web browser (Chrome, Firefox, Safari, Edge)
* Node.js v18+ (optional, for local development server)
* Supabase project credentials

### Installation
```bash
git clone https://github.com/itsgoharrehman/learnza-e-library.git
cd learnza-e-library
```

### Configuration
Configure your Supabase credentials in your environment or configuration script:
```javascript
const SUPABASE_URL = "https://your-project.supabase.co";
const SUPABASE_ANON_KEY = "your-anon-key";
```

### Running Locally
Serve the application using any static HTTP server:
```bash
npx serve .
```

## Repository Structure
```text
learnza-e-library/
├── assets/
│   ├── css/
│   ├── js/
│   └── icons/
├── admin/
│   ├── dashboard.html
│   └── manage-catalog.js
├── index.html
├── books.html
└── README.md
```

## Security Policy

If you discover a vulnerability or security flaw, please report it privately to `goharrehmanfsd260@gmail.com` instead of creating a public issue.

## Maintainer

* **Gohar Rehman**
* GitHub: [@itsgoharrehman](https://github.com/itsgoharrehman)
* Email: `goharrehmanfsd260@gmail.com`
* Website: [itsgoharrehman.netlify.app](https://itsgoharrehman.netlify.app/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
