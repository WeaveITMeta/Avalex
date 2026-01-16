# Avalex Website Plan

## Table of Contents
1. [Mission](#mission)
2. [The Simplest Solution](#the-simplest-solution)
3. [The Great Healthcare Plan](#the-great-healthcare-plan)
4. [Site Architecture](#site-architecture)
5. [Navigation Structure](#navigation-structure)
6. [Page Layouts](#page-layouts)
7. [Tech Stack: Rust + Leptos + Trunk + TailwindCSS](#tech-stack)
8. [Project Setup](#project-setup)
9. [Component Architecture](#component-architecture)
10. [Implementation](#implementation)

---

## Mission

**Global Wellbeing Through Local Empowerment**

The simplest solution for global healthcare is to empower individuals with knowledge, connect them with qualified integrative practitioners, and provide transparent, evidence-based pathways to wellness.

---

## The Simplest Solution

### Core Principle: Treat the Root Cause, Not Just Symptoms

```
EDUCATION → PREVENTION → INTEGRATION → ACCOUNTABILITY
```

### Three Pillars of Global Wellbeing

| Pillar | Description | Outcome |
|--------|-------------|---------|
| **Know** | Health literacy and self-education | Informed decisions |
| **Find** | Connect with qualified practitioners | Right care, right time |
| **Act** | Preventive and integrative approaches | Sustainable wellness |

### Why This Works
- **90%** of chronic disease is preventable through lifestyle
- **Integrative medicine** addresses root causes, not just symptoms
- **Local empowerment** reduces dependency on broken systems
- **Transparency** builds trust and accountability

---

## The Great Healthcare Plan {#the-great-healthcare-plan}

*Aligned with the Great Healthcare Plan announced January 2026*

### Core Principles

| Principle | Description | Implementation |
|-----------|-------------|----------------|
| **Price Transparency** | Full disclosure of all healthcare costs | Searchable price lists, provider comparisons |
| **Direct Payments** | Money directly to patients | Eligibility tools, payment calculators |
| **Drug Price Reduction** | Most-Favored-Nation pricing (80-90% savings) | TrumpRx integration, OTC alternatives |
| **Lower Premiums** | Competitive insurance marketplace | Side-by-side plan comparisons |
| **Plain English** | No confusing jargon | Clear explanations, claim denial stats |
| **Insurer Accountability** | Transparent rejection rates | Public accountability dashboards |
| **PBM Reform** | Eliminate kickbacks | Direct pricing, no middlemen |

### Key Features to Build

```
TRANSPARENCY TOOLS
├── Interactive price calculators
├── Searchable provider/insurer prices
├── Hospital price comparison
└── Procedure cost estimators

CONSUMER EMPOWERMENT
├── HSA guides and tools
├── Direct payment options
├── Premium estimators
├── Insurance plan comparisons
└── Claim rejection statistics

DRUG PRICING
├── Most-Favored-Nation comparisons
├── Generic alternatives finder
├── OTC options database
└── TrumpRx.gov integration

ACCOUNTABILITY
├── Insurer performance ratings
├── Provider quality scores
├── Plain-English breakdowns
└── Public reporting dashboards
```

---

## Site Architecture

### Primary Navigation (Dropdown Menus)

```
┌──────────────────────────────────────────────────────────────────────────────────────────┐
│  AVALEX                                                                                  │
├──────────────────────────────────────────────────────────────────────────────────────────┤
│  Home │ Healthcare Plan │ Price Transparency │ Drug Prices │ Practitioners │ Resources  │
└──────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## Navigation Structure

### 1. HOME
- Hero: "The Great Healthcare Plan — Direct Payments. Lowest Drug Prices. Full Transparency."
- Three pillars overview (Know, Find, Act)
- Quick links to key tools (Price Calculator, Drug Prices, Find Care)
- Key statistics and reform highlights

### 2. HEALTHCARE PLAN (Dropdown)
```
Healthcare Plan
├── Overview
│   └── The Great Healthcare Plan
├── Direct Payments
│   ├── Eligibility Calculator
│   └── How It Works
├── Lower Premiums
│   ├── Premium Estimator
│   └── Competition Benefits
├── Insurer Accountability
│   ├── Plain-English Explanations
│   └── Claim Denial Statistics
└── PBM Reform
    └── Eliminating Kickbacks
```

### 3. PRICE TRANSPARENCY (Dropdown)
```
Price Transparency
├── Price Calculator
├── Hospital Prices
├── Provider Search
├── Procedure Costs
├── Insurance Comparisons
│   ├── HMO vs PPO
│   └── Side-by-Side Plans
└── Problems We're Solving
    ├── Healthcare Costs
    ├── Access Gaps
    ├── Administrative Complexity
    ├── Quality & Safety
    └── Health Disparities
```

### 4. DRUG PRICES (Dropdown)
```
Drug Prices
├── Most-Favored-Nation Pricing
├── Drug Price Lookup
├── Generic Alternatives
├── OTC Options
├── TrumpRx.gov Integration
└── Prescription Savings Calculator
```

### 5. PRACTITIONERS (Dropdown)
```
Practitioners
├── Find Care (Provider Search)
├── Holistic Doctors
├── Naturopathic Physicians
├── Medical Doctors
├── Acupuncturists
├── Chiropractors
├── Clinical Nutritionists
├── Herbalists
├── Homeopaths
├── Immunologists
├── Massage Therapists
├── Physical Therapists
├── Psychologists
├── Registered Nurses
├── Surgeons
└── Colon Therapists
```

### 6. RESOURCES (Dropdown)
```
Resources
├── Consumer Tools
│   ├── HSA Guide
│   ├── Direct Payment Options
│   └── Cost Savings Tips
├── Philosophy
│   ├── Systems Theory
│   ├── Political Science
│   └── 5-Step Process
├── Prevention & Wellness
│   ├── Lifestyle Medicine
│   ├── Nutrition
│   └── Mental Wellness
├── Technology
│   ├── AI & Data
│   ├── Telehealth
│   └── Gene Editing (CRISPR)
├── External Links
│   ├── TrumpRx.gov
│   └── Healthcare.gov
└── About Avalex
    ├── Mission
    ├── Blog/News
    └── Contact
```

---

## Page Layouts

### Homepage Layout

```
┌─────────────────────────────────────────────────────────────────────┐
│                         NAVIGATION BAR                              │
│  AVALEX  │ Healthcare Plan │ Price Transparency │ Drug Prices │... │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    HERO SECTION (Gradient bg-indigo-600 → purple)   │
│                                                                     │
│              "The Great Healthcare Plan"                            │
│    "Direct payments. Lowest drug prices in the world.               │
│                   Full transparency."                               │
│                                                                     │
│        [Get Your Direct Payment]  [Check Drug Prices]               │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│    ┌─────────────┐  ┌─────────────┐  ┌─────────────┐               │
│    │    KNOW     │  │    FIND     │  │     ACT     │               │
│    │  Education  │  │ Practitioners│  │  Prevention │               │
│    │  & Literacy │  │  & Experts  │  │  & Wellness │               │
│    └─────────────┘  └─────────────┘  └─────────────┘               │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    KEY REFORM HIGHLIGHTS                            │
│    80-90% Drug Savings │ Direct Payments │ Price Transparency       │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    INTERACTIVE TOOLS                                │
│    [Price Calculator] [Drug Lookup] [Insurance Comparison]          │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    KEY STATISTICS                                   │
│    $4.1T spent │ 28M uninsured │ 250K preventable deaths           │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    FEATURED PRACTITIONERS                           │
│    [Dr. Mark Hyman] [Dr. Joseph Pizzorno] [Dr. Frank Lipman]       │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                         FOOTER                                      │
└─────────────────────────────────────────────────────────────────────┘
```

### Dropdown Menu Component

```html
<!-- Example Dropdown Structure -->
<nav class="navbar">
  <div class="dropdown">
    <button class="dropdown-toggle">Problems</button>
    <ul class="dropdown-menu">
      <li><a href="/problems/costs">Healthcare Costs</a></li>
      <li><a href="/problems/access">Access Gaps</a></li>
      <li><a href="/problems/complexity">Administrative Complexity</a></li>
      <!-- ... more items -->
    </ul>
  </div>
</nav>
```

### Content Page Layout

```
┌─────────────────────────────────────────────────────────────────────┐
│                         NAVIGATION BAR                              │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  BREADCRUMB: Home > Solutions > Philosophy > Systems Theory         │
│                                                                     │
├───────────────────────────────────────┬─────────────────────────────┤
│                                       │                             │
│         MAIN CONTENT                  │      SIDEBAR                │
│                                       │                             │
│  # Page Title                         │  Quick Links                │
│                                       │  ─────────────              │
│  Content from .md files               │  Related Topics             │
│  rendered as HTML                     │  Featured Doctors           │
│                                       │  Resources                  │
│                                       │                             │
├───────────────────────────────────────┴─────────────────────────────┤
│                         FOOTER                                      │
└─────────────────────────────────────────────────────────────────────┘
```

### Practitioner Directory Layout

```
┌─────────────────────────────────────────────────────────────────────┐
│                         NAVIGATION BAR                              │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  FILTER BAR: [Specialty ▼] [Location ▼] [Approach ▼] [Search...]   │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  │
│  │  Dr. Mark Hyman  │  │ Dr. Frank Lipman │  │ Dr. Kelly Brogan │  │
│  │  Functional Med  │  │  Integrative     │  │  Holistic Psych  │  │
│  │  [View Profile]  │  │  [View Profile]  │  │  [View Profile]  │  │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘  │
│                                                                     │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  │
│  │ Dr. J. Pizzorno  │  │ Dr. Alan Gaby    │  │ Dr. Leo Galland  │  │
│  │  Naturopathic    │  │  Nutritional Med │  │  Functional Med  │  │
│  │  [View Profile]  │  │  [View Profile]  │  │  [View Profile]  │  │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘  │
│                                                                     │
├─────────────────────────────────────────────────────────────────────┤
│                         FOOTER                                      │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Tech Stack: Rust + Leptos + Trunk + TailwindCSS {#tech-stack}

### Why This Stack?

| Technology | Purpose | Benefit |
|------------|---------|---------|
| **Rust** | Core language | Safety, speed, reliability for sensitive health data |
| **Leptos** | Reactive UI framework | High-performance SSR + hydration, SEO-friendly |
| **Trunk** | WASM bundler | Simplified build and deployment |
| **TailwindCSS** | Styling | Rapid prototyping, mobile-first, accessible |

### Stack Advantages

- **Performance**: Leptos enables SSR + hydration ideal for public-facing healthcare site
- **Security**: Rust's memory safety crucial for handling health-related data/tools
- **SEO**: Server-side rendering ensures search engine visibility
- **Speed**: WASM compilation delivers near-native performance
- **Accessibility**: TailwindCSS + @tailwindcss/forms for WCAG compliance

---

## Project Setup {#project-setup}

### Prerequisites

```bash
# 1. Install Rust (nightly for Leptos)
rustup toolchain install nightly
rustup default nightly
rustup target add wasm32-unknown-unknown

# 2. Install Trunk and cargo-generate
cargo install --locked trunk
cargo install --locked cargo-generate
```

### Create Project

```bash
# Create new Leptos project
cargo new avalex --lib
cd avalex

# Add dependencies to Cargo.toml
cat >> Cargo.toml <<EOF
[dependencies]
leptos = { version = "0.7", features = ["csr", "nightly"] }
leptos_router = "0.7"
console_error_panic_hook = "0.1"
wasm-bindgen = "0.2"

[profile.release]
codegen-units = 1
lto = true
opt-level = "z"
EOF
```

### TailwindCSS Setup

```bash
# Initialize npm and install Tailwind
npm init -y
npm install -D tailwindcss @tailwindcss/forms postcss autoprefixer
npx tailwindcss init

# Create input.css
mkdir -p style
cat > style/input.css <<EOF
@tailwind base;
@tailwind components;
@tailwind utilities;
EOF
```

### tailwind.config.js

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.rs", "./index.html"],
  theme: { extend: {} },
  plugins: [require("@tailwindcss/forms")],
};
```

### index.html (Trunk Entry)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Avalex – The Great Healthcare Plan</title>
  <link data-trunk rel="css" href="style/output.css" />
  <link data-trunk rel="rust" data-type="module" />
</head>
<body></body>
</html>
```

### Development Workflow

```bash
# Terminal 1 – Tailwind watch
npx tailwindcss -i ./style/input.css -o ./style/output.css --watch

# Terminal 2 – Trunk dev server
trunk serve --open
```

Hot-reloading Leptos app at `http://localhost:8080`

---

## Component Architecture {#component-architecture}

### Project Structure

```
src/
├── components/
│   ├── Header.rs          # Sticky nav with dropdowns
│   ├── Footer.rs          # 4-column footer
│   ├── Hero.rs            # "The Great Healthcare Plan" hero
│   ├── PriceCalculator.rs # Interactive price tool
│   ├── DrugLookup.rs      # Drug price search
│   ├── InsuranceCompare.rs# Side-by-side plans
│   ├── PractitionerCard.rs# Doctor profile cards
│   └── ContactForm.rs     # Server function for inquiries
├── pages/
│   ├── Home.rs
│   ├── HealthcarePlan.rs
│   ├── DirectPayments.rs
│   ├── PriceTransparency.rs
│   ├── DrugPrices.rs
│   ├── Practitioners.rs
│   └── Resources.rs
├── app.rs                 # Main app with Router
├── main.rs
└── lib.rs
style/
├── input.css
└── output.css
index.html
Cargo.toml
tailwind.config.js
```

### Basic App Structure (src/lib.rs)

```rust
use leptos::*;
use leptos_router::*;

#[component]
pub fn App() -> impl IntoView {
    view! {
        <Router>
            <div class="min-h-screen bg-gray-50">
                <Header/>
                <main>
                    <Routes>
                        <Route path="/" view=Home/>
                        <Route path="/healthcare-plan" view=HealthcarePlan/>
                        <Route path="/direct-payments" view=DirectPayments/>
                        <Route path="/price-transparency" view=PriceTransparency/>
                        <Route path="/drug-prices" view=DrugPrices/>
                        <Route path="/practitioners" view=Practitioners/>
                        <Route path="/resources" view=Resources/>
                    </Routes>
                </main>
                <Footer/>
            </div>
        </Router>
    }
}

#[component]
pub fn main() {
    mount_to_body(|| view! { <App/> });
}
```

### Hero Component Example

```rust
#[component]
pub fn Hero() -> impl IntoView {
    view! {
        <section class="bg-gradient-to-r from-indigo-600 to-purple-700 text-white py-20">
            <div class="max-w-7xl mx-auto text-center px-4">
                <h1 class="text-5xl font-extrabold mb-6">
                    "The Great Healthcare Plan"
                </h1>
                <p class="text-xl mb-8">
                    "Direct payments. Lowest drug prices in the world. Full transparency."
                </p>
                <div class="flex justify-center gap-4">
                    <a href="/direct-payments" 
                       class="bg-white text-indigo-700 px-8 py-4 rounded-lg font-bold text-lg hover:bg-gray-100">
                        "Get Your Direct Payment"
                    </a>
                    <a href="/drug-prices"
                       class="border-2 border-white text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-white/10">
                        "Check Drug Prices"
                    </a>
                </div>
            </div>
        </section>
    }
}
```

### Header Component with Dropdowns

```rust
#[component]
pub fn Header() -> impl IntoView {
    view! {
        <header class="bg-indigo-700 text-white shadow-lg sticky top-0 z-50">
            <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="flex justify-between h-16">
                    <div class="flex items-center">
                        <a href="/" class="text-2xl font-bold">"Avalex"</a>
                    </div>
                    <div class="hidden md:flex items-center space-x-4">
                        <NavDropdown title="Healthcare Plan" items=vec![
                            ("Overview", "/healthcare-plan"),
                            ("Direct Payments", "/direct-payments"),
                            ("Lower Premiums", "/premiums"),
                        ]/>
                        <NavDropdown title="Price Transparency" items=vec![
                            ("Price Calculator", "/price-calculator"),
                            ("Hospital Prices", "/hospital-prices"),
                            ("Insurance Compare", "/insurance-compare"),
                        ]/>
                        <NavDropdown title="Drug Prices" items=vec![
                            ("Drug Lookup", "/drug-prices"),
                            ("Generic Alternatives", "/generics"),
                            ("OTC Options", "/otc"),
                        ]/>
                        <NavDropdown title="Practitioners" items=vec![
                            ("Find Care", "/find-care"),
                            ("Holistic Doctors", "/practitioners/holistic"),
                            ("All Specialties", "/practitioners"),
                        ]/>
                        <a href="/resources" class="hover:text-indigo-200">"Resources"</a>
                    </div>
                </div>
            </nav>
        </header>
    }
}
```

---

## Implementation

### Content Mapping

| Source File | Website Section |
|-------------|-----------------|
| `README.md` | Problems pages |
| `Philosophy/SystemsTheory.md` | Solutions > Philosophy |
| `Philosophy/PoliticalScience.md` | Solutions > Philosophy |
| `Philosophy/5StepProcess.md` | Solutions > Philosophy |
| `Philosophy/TheAmericanHealthcareSystem.md` | Solutions > Philosophy |
| `CRISPER/GeneEditing.md` | Solutions > Technology |
| `Professions/Doctors/Holistic/*.md` | Practitioners > Holistic Doctors |
| `Professions/*/` | Practitioners subpages |
| `Resources/` | Resources subpages |

### Dropdown Menu CSS (Simple Implementation)

```css
/* Simple dropdown with CSS only */
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-menu {
  display: none;
  position: absolute;
  background: white;
  min-width: 200px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  border-radius: 8px;
  padding: 8px 0;
  z-index: 100;
}

.dropdown:hover .dropdown-menu {
  display: block;
}

.dropdown-menu li {
  padding: 8px 16px;
}

.dropdown-menu li:hover {
  background: #f5f5f5;
}
```

---

## Footer Structure

### 4-Column Footer Layout

```
┌─────────────────────────────────────────────────────────────────────┐
│                         FOOTER (dark bg)                            │
├────────────────┬────────────────┬────────────────┬──────────────────┤
│  NAVIGATION    │  TRANSPARENCY  │  FOR CONSUMERS │  LEGAL & CONTACT │
│                │                │                │                  │
│  Home          │  Price Tools   │  Drug Prices   │  Privacy Policy  │
│  Healthcare    │  Insurer       │  Insurance     │  Terms of Use    │
│    Plan        │  Accountability│  HSA Guide     │  Accessibility   │
│  Practitioners │  Provider      │  Direct        │  Disclaimer      │
│  Resources     │  Pricing       │  Payments      │  Contact Us      │
│  About         │                │                │                  │
│  Blog/News     │                │                │  [Social Icons]  │
├────────────────┴────────────────┴────────────────┴──────────────────┤
│  © 2026 Avalex – Built with Rust + Leptos + TailwindCSS             │
│  TrumpRx.gov | Healthcare.gov                                       │
└─────────────────────────────────────────────────────────────────────┘
```

### Footer Component

```rust
#[component]
pub fn Footer() -> impl IntoView {
    view! {
        <footer class="bg-gray-900 text-gray-300 py-12">
            <div class="max-w-7xl mx-auto px-4 grid grid-cols-1 md:grid-cols-4 gap-8">
                // Column 1: Navigation
                <div>
                    <h3 class="text-white font-bold mb-4">"Navigation"</h3>
                    <ul class="space-y-2">
                        <li><a href="/" class="hover:text-white">"Home"</a></li>
                        <li><a href="/healthcare-plan" class="hover:text-white">"Healthcare Plan"</a></li>
                        <li><a href="/practitioners" class="hover:text-white">"Practitioners"</a></li>
                        <li><a href="/resources" class="hover:text-white">"Resources"</a></li>
                    </ul>
                </div>
                // Column 2: Transparency
                <div>
                    <h3 class="text-white font-bold mb-4">"Transparency"</h3>
                    <ul class="space-y-2">
                        <li><a href="/price-transparency" class="hover:text-white">"Price Tools"</a></li>
                        <li><a href="/accountability" class="hover:text-white">"Insurer Accountability"</a></li>
                        <li><a href="/provider-pricing" class="hover:text-white">"Provider Pricing"</a></li>
                    </ul>
                </div>
                // Column 3: For Consumers
                <div>
                    <h3 class="text-white font-bold mb-4">"For Consumers"</h3>
                    <ul class="space-y-2">
                        <li><a href="/drug-prices" class="hover:text-white">"Drug Prices"</a></li>
                        <li><a href="/insurance-compare" class="hover:text-white">"Insurance Tools"</a></li>
                        <li><a href="/hsa-guide" class="hover:text-white">"HSA Guide"</a></li>
                    </ul>
                </div>
                // Column 4: Legal
                <div>
                    <h3 class="text-white font-bold mb-4">"Legal"</h3>
                    <ul class="space-y-2">
                        <li><a href="/privacy" class="hover:text-white">"Privacy Policy"</a></li>
                        <li><a href="/terms" class="hover:text-white">"Terms of Use"</a></li>
                        <li><a href="/contact" class="hover:text-white">"Contact Us"</a></li>
                    </ul>
                </div>
            </div>
            <div class="max-w-7xl mx-auto px-4 mt-8 pt-8 border-t border-gray-700 text-center">
                <p>"© 2026 Avalex – Built with Rust + Leptos + TailwindCSS"</p>
            </div>
        </footer>
    }
}
```

---

## Build & Deploy

### Build Commands

```bash
# Development
trunk serve --open

# Production build
trunk build --release

# Output: dist/ folder with static files + WASM
```

### Deployment Options

| Platform | Command | Notes |
|----------|---------|-------|
| **Netlify** | Drag dist/ or connect repo | Auto-builds with trunk |
| **Vercel** | `vercel --prod` | Configure build command |
| **Cloudflare Pages** | Connect repo | Fast global CDN |
| **GitHub Pages** | Push dist/ to gh-pages | Free hosting |

---

## Phase Rollout

| Phase | Scope | Timeline |
|-------|-------|----------|
| **1** | Project setup + Homepage + Navigation | Week 1 |
| **2** | Healthcare Plan pages + Direct Payments | Week 2 |
| **3** | Price Transparency tools + Drug Prices | Week 3 |
| **4** | Practitioners directory (45+ profiles) | Week 4 |
| **5** | Resources + Search + Contact forms | Week 5 |
| **6** | Polish, accessibility audit, deploy | Week 6 |

---

## Summary

**The simplest solution for global wellbeing:**

1. **Educate** - Provide clear, evidence-based health information
2. **Connect** - Link people with qualified integrative practitioners
3. **Empower** - Enable local, preventive, root-cause approaches
4. **Transparency** - Full price disclosure and accountability

**Website delivers this through:**
- **Rust + Leptos + TailwindCSS** for performance, safety, and beautiful UI
- Clean navigation with dropdown menus
- Interactive tools: Price Calculator, Drug Lookup, Insurance Comparison
- Content organized by Healthcare Plan → Transparency → Drug Prices → Practitioners → Resources
- Mobile-responsive, WCAG-accessible design
- Existing .md content as data source
- Aligned with the Great Healthcare Plan (January 2026)

**Avalex: The best healthcare website in the world.** 🚀

---

*Document Version: 2.0*
*Created: January 2026*
*Tech Stack: Rust + Leptos 0.7 + Trunk + TailwindCSS*
