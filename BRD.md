# Business Requirements Document (BRD)
## altpay - Nigerian Payment Gateway

---

## Document Information
| Field | Details |
|-------|---------|
| **Project Name** | altpay Payment Gateway |
| **Version** | 1.0 |
| **Date** | January 30, 2026 |
| **Status** | Draft |

---

## 1. Executive Summary

### 1.1 Purpose
This document outlines the business requirements for altpay, a Nigerian payment gateway designed to help businesses accept payments easily, securely, and reliably. The platform is built to support fast transactions and transparent pricing for Nigerian SMEs and startups.

### 1.2 Project Overview
altpay is a payment solution that:
- Simplifies business incorporation in Nigeria
- Offers corporate bank accounts through partnership with alt bank
- Provides a secure payment gateway with competitive pricing
- Enables next-day settlement for merchants

### 1.3 Key Value Propositions
- **Trusted Platform**: Trusted by over 10 businesses
- **Industry-leading**: Transaction success rates
- **Affordable**: 1.5% per transaction, capped at ₦2,000
- **Fast Settlement**: Next business day settlement
- **Local Focus**: Designed specifically for Nigerian businesses

---

## 2. Target Audience

### 2.1 Primary Audience
Nigerian SMEs and startups including:
- Online retailers
- Freelancers
- Small merchants
- Businesses handling 1,000-10,000 transactions monthly
- Businesses prioritizing low costs and easy setup

### 2.2 Secondary Audience
E-commerce platforms including:
- altmall
- altpower
- altmobile
- WooCommerce integrations
- Shopify integrations
- Other e-commerce platforms

---

## 3. Product Features

### 3.1 Current Features

#### 3.1.1 Card Payments
- Accept card payments from customers (Visa, Mastercard, Verve)
- Enter card details to make full payment
- Card number, expiry date (MM/YY), and CVV input
- "Remember this card" functionality (secure tokenization)
- Multi-currency support (Nigeria flag/currency selector)
- **3D Secure 2.0** authentication for enhanced security
- Real-time fraud detection and prevention

#### 3.1.2 Security Features
- PCI DSS Level 1 compliant payment processing
- Card tokenization (raw card data never stored)
- TLS 1.3 encryption for all data transmission
- Fraud prevention with risk scoring
- IP-based velocity checks
- Device fingerprinting

#### 3.1.3 Developer Tools
- RESTful API for custom integrations
- Webhooks for real-time event notifications
- Test/Sandbox environment for development
- API documentation and SDKs (PHP, JavaScript, Python)
- Publishable and Secret API keys (Stripe-like)

### 3.2 Coming Soon Features

#### 3.2.1 Payment Links
- Generate payment links to sell online and get paid
- Sell online without a website
- Receive instant payments from customers using payment links
- Customizable payment pages
- Expiration dates for time-limited offers
- QR code generation for offline sharing

#### 3.2.2 Recurring Payments
- Tokenize cards for recurring payments
- Subscription billing support
- Flexible billing cycles (daily, weekly, monthly, yearly)
- Automatic retry for failed payments
- Dunning management (failed payment notifications)
- Subscription lifecycle webhooks

#### 3.2.3 Pay with Credit
- Applicable to AltBank accounts only
- Credit-based payment options
- Pre-approval and credit limit management

#### 3.2.4 Installment Payments
- Make installment payments
- Split payment functionality
- Configurable installment plans (2, 3, 6, 12 months)
- Interest calculation options

#### 3.2.5 Refunds & Disputes
- Full and partial refund processing
- Automated refund to original payment method
- Chargeback/dispute management dashboard
- Evidence submission for dispute resolution
- Dispute outcome tracking

---

## 4. How It Works

### 4.1 Integration Flow
1. **Connect altpay**: Integrate altpay into your website, app, or checkout flow using our APIs or SDKs
2. **Accept payments**: Customers complete payments seamlessly with 3D Secure protection
3. **Get settled**: Funds are processed and paid to your bank account the next business day

### 4.2 Payment Flow
- Customer selects payment method
- Enters payment details (Amount, First Name, Last Name, Email)
- Completes card details (Card Number, Valid Till, CVV)
- 3D Secure verification (if required based on risk assessment)
- Payment is processed securely with real-time fraud checks
- Customer receives confirmation
- Merchant receives webhook notification
- Merchant receives settlement next business day

### 4.3 Integration Options
| Option | Description | Best For |
|--------|-------------|----------|
| **Redirect Checkout** | Customer redirected to altpay-hosted page | Quick setup, minimal coding |
| **Embedded Checkout** | Payment form embedded in merchant's site | Seamless user experience |
| **Custom Integration** | Full API access for custom UI | Complete control over UX |

---

## 5. Business Registration Services

### 5.1 Overview
altpay and bold by alt simplify business incorporation in Nigeria and offer corporate bank accounts.

### 5.2 Benefits of Incorporation
- Faster payouts
- Increased transfer limits
- Access to POS terminals
- Additional business services

### 5.3 Registration Types & Pricing

| Registration Type | Price | Timeline |
|-------------------|-------|----------|
| Tax Identification Number | ₦3,500 | 7-9 days |
| Business Name Registration (Sole Proprietorship) | ₦35,000 | 7-9 days |
| Limited Liability Company Registration | ₦65,000 | 7-9 days |
| Limited Partnership Registration | ₦55,000 | 7-9 days |
| Limited Liability Partnership Registration | ₦75,000 | 7-9 days |
| Non-Governmental Organization Registration | ₦140,000 | 6-8 weeks |

---

## 6. Pricing Structure

### 6.1 Transaction Fees
- **Rate**: 1.5% per transaction
- **Cap**: ₦2,000 maximum fee per transaction
- **Hidden Fees**: None

### 6.2 Settlement Timeline
- Next business day settlement to merchant's bank account

---

## 7. Site Architecture

### 7.1 Sitemap Structure

```
altpay
├── Home
│   ├── Hero Section
│   ├── Why altpay
│   ├── How it works
│   ├── Testimonials
│   └── Support
│
├── Why altpay?
│   ├── Overview
│   ├── Key Benefits
│   └── Call to Action
│
├── Products
│   └── Payment Gateway
│       ├── Card
│       └── Coming Soon:
│           ├── Recurring Payment
│           ├── Pay with Credit
│           └── Installment Payment
│
├── Developers
│   ├── Getting Started - APIs & SDKs
│   ├── Integration Guides (API Documentation)
│   ├── Code Samples
│   └── Developer Support
│
├── Pricing
│   ├── Pricing Overview
│   ├── Transaction Fees (1.5% capped at ₦2,000)
│   ├── Settlement Timeline
│   ├── No Hidden Fees (Explanation in details)
│   └── CTA: Get Started
│
├── Testimonials
│   ├── Merchant Stories (SMEs)
│   ├── Growth & Success Metrics
│   └── Logos / Social Proof
│
└── Support
    ├── Help Center / FAQs
    ├── Contact Support
    └── Documentation Links
```

### 7.2 Navigation Bar
Home | Why altpay | Products | Developers | Pricing | Testimonials | Support

---

## 8. Page Wireframes

### 8.1 Home Page

#### Hero Section
- **Headline**: "The Smart Way to Accept Payments in Nigeria / Get paid seamlessly, everyday."
- **Sub-headline**: "Accept payments from customers across Nigeria with speed, reliability, and pricing that makes sense."
- **CTA**: "Start accepting payments"

#### Visual Guidelines
- **Hero Section (All Audiences)**: Real merchant paying with card with light UI overlay showing "Payment Successful", dashboard metrics, or transaction flow
- **SME-Focused Section**: Online sellers holding a tablet with "Happy merchant receiving payments"
- **Developer Section**: Laptop screen showing clean code snippets + payment dashboard. Split-screen style: code on one side, live transaction UI on the other

### 8.2 Why altpay Section

**Introduction**: altpay makes it easy to accept payments without the usual stress. We help businesses get paid faster with affordable pricing, reliable processing, and next-day settlement, all built on an infrastructure you can trust.

**Target Statement**: Whether you're a startup, SME, or scaling enterprise, altpay helps you get paid without delays.

#### Key Benefits
| Benefit | Description |
|---------|-------------|
| **Affordable pricing** | 1.5% per transaction, capped at ₦2,000. No hidden fees. |
| **Fast, reliable payments** | Built on stable infrastructure to keep transactions flowing smoothly. |
| **Next-day settlement** | Access your funds the next business day. |
| **Built for local businesses** | Designed with Nigerian businesses in mind, and ready to grow with you. |

---

## 9. Testimonials

### 9.1 Customer Testimonials

> "We were able to set things up without any back-and-forth. We also started receiving settlements the next business day."
> — **Product Manager, altpower**

> "altpay is consistent, fast, and dependable. We needed a payment solution that could handle peak traffic without hiccups. altpay has delivered from day one."
> — **COO, Onifila Couture**

> "The process is clear, the experience is smooth, and settlements happen when they're expected. It's straightforward and dependable."

### 9.2 Testimonials Section Design
- **Format**: Short quotes with profile pictures, names & portfolio
- **Look**: Carousel or grid of real client feedback with photos
- **Feel**: Builds social proof and client confidence

---

## 10. FAQs

### Q: What is altpay?
**A**: altpay is a Nigerian payment gateway that helps businesses accept payments easily, securely, and reliably. It is built to support fast transactions and transparent pricing.

### Q: How does altpay work?
**A**: altpay integrates with your website or app and lets you collect payments via secure payment links or embedded checkout. Once a payment is successful, your funds are settled to your bank account the next business day.

*Link to additional FAQs*

---

## 11. Contact Information

### 11.1 Contact Form Fields
- Name
- Email
- Phone number
- Message
- Business Name
- About Business

### 11.2 Contact Details
- **Email**: help@altbank.ng
- **Phone**: 02017000555
- **Address**: The alternative bank - 22 Marina, Lagos Island, Lagos

---

## 12. SEO & Technical Requirements

### 12.1 Technical Foundation & Core Setup

#### Objectives
- Ensure the platform is high-performing, secure, and discoverable by Nigerian merchants

#### Requirements
| Requirement | Details |
|-------------|---------|
| **Performance & Mobile-First** | Optimize for speed to support "clean, modern design" and ensure site is fully responsive for SMEs who manage businesses via mobile |
| **Security Architecture** | Implement sitewide HTTPS and follow security best practices for processing "Cards" and "Recurring Payments" to build trust and reliability |
| **SEO-Friendly URL Structure** | Use clean, descriptive slugs: /pricing, /developers, /business-registration |

#### Metadata Implementation
- **Home Page Title**: altpay | Secure Payment Gateway for Nigerian Businesses
- **Description**: Accept payments with 1.5% fees (capped at ₦2,000). Get next-day settlement and seamless API integration.

### 12.2 Content Strategy & Merchant Funnels

#### Objectives
- Use business registration and learning resources to attract and convert unregistered merchants

#### Requirements
| Requirement | Details |
|-------------|---------|
| **Strategic Blog Integration** | Build a blog within a subfolder (e.g., /blog) to host guides and insights mentioned in learning resources |
| **Business Registration Funnel** | Optimize pages for terms like "Business Name Registration" (₦35k) and "LLC Registration" (₦65k). Link directly to "Start accepting payments" CTA |
| **FAQ Schema** | Implement FAQ Schema for "What is altpay?" section |
| **Financial Service Schema** | Implement to help pricing and features appear as rich snippets in Google search results |
| **Testimonial Markup** | Code testimonial section using crawlable text (not just images) for social proof |

### 12.3 Developer-Centric SEO & Local Authority

#### Objectives
- Rank for technical keywords to attract developers and establish local trust in the Nigerian market

#### Requirements
| Requirement | Details |
|-------------|---------|
| **Indexable Developer Portal** | Ensure "APIs & SDKs" and "Integration Guides" are in text-based format that search engines can crawl |
| **Local SEO & Trust Signals** | Include Lagos Island/Head office address and support contact (help@altbank.ng) in footer for local "near me" business searches |
| **Feature-Specific Landing Pages** | Create dedicated, SEO-optimized sections for upcoming features like "Pay with Credit" and "Installment Payment" |
| **Dynamic Sitemap** | Maintain an XML sitemap including all pages: Home, Why altpay, Products, Developers, Pricing, Testimonials, and Support |

### 12.4 Learning Resources
- Blog
- Guides
- Video tutorials
- Decode Fintech podcast/newsletter for business insights

---

## 13. Product Visuals and Identity

### 13.1 Design Guidelines
1. **Clean, modern design** focused on simplicity, speed, and effortless navigation to drive conversions
2. **Bold, confidence-inspiring brand colors** that communicate trust, security, and reliability at every touchpoint
3. **Authentic, real-life visuals** highlighting businesses accepting payments seamlessly and customers enjoying smooth checkout experiences
4. **Contemporary, professional typography** that enhances readability while reinforcing a strong, credible brand presence

### 13.2 Brand Colors
- Primary: Purple (#A020F0 or similar)
- Secondary: Deep Blue/Indigo for "pay" in logo
- Accent colors for UI elements

---

## 14. Functional Requirements Summary

### 14.1 Payment Processing
- [ ] Card payment acceptance
- [ ] Multi-currency display (NGN primary)
- [ ] Secure card data entry (Card Number, Expiry, CVV)
- [ ] Save card functionality
- [ ] Transaction amount display
- [ ] Customer information capture (First Name, Last Name, Email)

### 14.2 Merchant Features
- [ ] Next-day settlement processing
- [ ] Dashboard for transaction monitoring
- [ ] Integration APIs and SDKs
- [ ] Payment link generation (Coming Soon)
- [ ] Recurring payment setup (Coming Soon)
- [ ] Installment payment options (Coming Soon)

### 14.3 Business Registration
- [ ] Tax ID registration
- [ ] Business name registration
- [ ] LLC registration
- [ ] Partnership registration
- [ ] NGO registration

### 14.4 Support
- [ ] Help center / FAQs
- [ ] Contact form
- [ ] Email support (help@altbank.ng)
- [ ] Phone support (02017000555)
- [ ] Developer documentation

### 14.5 Security & Fraud Prevention
- [ ] 3D Secure 2.0 integration
- [ ] Card tokenization (PCI-compliant vault)
- [ ] Real-time fraud detection
- [ ] Velocity checks (transaction limits per card/IP)
- [ ] Device fingerprinting
- [ ] Geolocation verification
- [ ] Chargeback/dispute management
- [ ] Multi-factor authentication for merchants

### 14.6 Developer Experience
- [ ] REST API documentation
- [ ] SDK libraries (PHP, JavaScript, Python)
- [ ] Webhook notifications
- [ ] Test/Sandbox environment
- [ ] API key management (publishable/secret keys)
- [ ] Code samples and integration guides
- [ ] API versioning

---

## 15. Non-Functional Requirements

### 15.1 Performance
| Requirement | Target |
|-------------|--------|
| Page load time | < 3 seconds |
| API response time (p95) | < 500ms |
| Payment processing time | < 3 seconds |
| Concurrent transactions | 10,000+ |
| Mobile-first design | 100% responsive |

### 15.2 Security
| Requirement | Standard |
|-------------|----------|
| **PCI DSS** | Level 1 compliance (highest) |
| **Data Encryption** | TLS 1.3 (in transit), AES-256 (at rest) |
| **Card Storage** | Tokenization only (never store raw PAN) |
| **CVV** | Never stored |
| **Authentication** | MFA for merchant accounts |
| **API Security** | Rate limiting, IP whitelisting |
| **Fraud Prevention** | Real-time risk scoring, 3DS 2.0 |
| **Audit Logging** | All transactions and admin actions logged |

### 15.3 Availability & Reliability
| Requirement | Target |
|-------------|--------|
| Uptime SLA | 99.9% |
| Recovery Time Objective (RTO) | < 1 hour |
| Recovery Point Objective (RPO) | < 5 minutes |
| Failover | Automatic processor failover |
| Data backup | Continuous with 7-year retention |

### 15.4 Compliance & Regulatory
| Requirement | Details |
|-------------|---------|
| **CBN Guidelines** | Central Bank of Nigeria payment regulations |
| **NDPR** | Nigeria Data Protection Regulation compliance |
| **PCI DSS** | Payment Card Industry Data Security Standard |
| **AML/KYC** | Anti-Money Laundering / Know Your Customer |

---

## 16. Appendix

### 16.1 Glossary
| Term | Definition |
|------|------------|
| **SME** | Small and Medium Enterprise |
| **CVV** | Card Verification Value |
| **API** | Application Programming Interface |
| **SDK** | Software Development Kit |
| **POS** | Point of Sale |
| **LLC** | Limited Liability Company |
| **NGO** | Non-Governmental Organization |
| **PCI DSS** | Payment Card Industry Data Security Standard |
| **3DS** | 3D Secure (card authentication protocol) |
| **TLS** | Transport Layer Security |
| **MFA** | Multi-Factor Authentication |
| **NDPR** | Nigeria Data Protection Regulation |
| **CBN** | Central Bank of Nigeria |
| **KYC** | Know Your Customer |
| **AML** | Anti-Money Laundering |

### 16.2 References
- altpay Product Documentation
- alt bank Partnership Materials
- Nigerian Business Registration Guidelines
- PCI Security Standards Council: https://www.pcisecuritystandards.org/
- CBN Payment System Guidelines

---

*End of Document*
