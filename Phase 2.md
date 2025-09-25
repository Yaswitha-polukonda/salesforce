```
+----------------------------------------------------------------------------------------------------+
| E-commerce CRM Project                                                                             |
|                                                                                                    |
| Phase 2: Org Setup & Configuration                                                                 |
| Salesforce Editions                                                                                |
| For the E-commerce CRM project, the Developer Edition is used for experimentation, testing, and learning. |
| In a real production scenario, Enterprise Edition would be ideal as it supports advanced customization, API integrations, and scalability. |
| This ensures our CRM can handle customer orders, loyalty programs, and marketing automation efficiently. |
|                                                                                                    |
|                                                                                                    |
|                                                                                                    |
| Company Profile Setup                                                                              |
| Company settings include entering the E-commerce company's legal name, address, default time zone, currency, and locale. |
| This ensures accurate reporting, multi-currency transactions, and a unified identity across the platform. |
| For example, setting default currency as INR/USD for international transactions and English as the default language. |
|                                                                                                    |
|                                                                                                    |
| Business Hours & Holidays                                                                          |
| Customer support in e-commerce requires defined business hours (e.g., 9 AM – 9 PM IST).            |
| Defining holidays like national holidays or festive breaks ensures SLA tracking for customer cases. |
| Escalations respect these working hours, preventing false SLA breaches.                            |
|                                                                                                    |
|                                                                                                    |
| Fiscal Year Settings                                                                               |
| E-commerce companies may follow either a standard fiscal year (Jan–Dec) or a custom fiscal year (Apr–Mar). |
| Aligning fiscal year is critical for sales forecasting, revenue reporting, and performance dashboards. |
|                                                                                                    |
|                                                                                                    |
| User Setup & Licenses                                                                              |
| Users such as Sales Managers, Marketing Specialists, and Customer Support Agents are created with unique logins. |
| Appropriate Salesforce licenses (Salesforce, Platform, or Chatter) are assigned based on their responsibilities. |
| For example, a support agent might only need Service Cloud functionality while a marketer requires campaign features. |
|                                                                                                    |
|                                                                                                    |
|                                                                                                    |
| Profiles                                                                                           |
| Profiles define the baseline permissions.                                                          |
| For this project, profiles such as System Administrator, Sales Profile, Marketing Profile, and Support Profile are customized. |
| Each profile ensures users only access data relevant to their job role.                            |
|                                                                                                    |
|                                                                                                    |
| Roles                                                                                              |
| A role hierarchy ensures data visibility matches organizational structure.                         |
| For e-commerce: CEO/Admin → Sales Manager → Sales Reps → Customer Support Agents.                  |
| Managers can see their team’s opportunities, but agents can only view their own.                   |
|                                                                                                    |
| Permission Sets:Permission sets grant additional privileges without changing the base profile.For example: |
|                                                                                                    |
|                                                                                                    |
| OWD (Organization-Wide Defaults)                                                                   |
| OWD determines baseline data visibility.                                                           |
| For the E-commerce CRM:                                                                            |
| Customer Data = Private                                                                            |
| Orders = Private                                                                                   |
| Product Catalog = Public Read Only                                                                 |
| This ensures sensitive data is protected while product data remains accessible for all teams.      |
|                                                                                                    |
| Sharing Rules                                                                                      |
| Sharing rules open up access where collaboration is needed.                                        |
| For example:                                                                                       |
| Regional sales teams may be allowed to share opportunities across a territory.                     |
| Support teams may be given read-only access to order history to resolve customer queries.          |
|                                                                                                    |
|                                                                                                    |
| Login Access Policies                                                                              |
| Security policies include:                                                                         |
| IP restrictions (restricting logins to office networks)                                            |
| Login hours (blocking access outside work shifts)                                                  |
| Two-factor authentication                                                                          |
| These measures protect sensitive e-commerce data from unauthorized access.                         |
|                                                                                                    |
|                                                                                                    |
| Dev Org Setup                                                                                      |
| The Developer Org is used for all configuration and customization first.                           |
| Objects for Orders, Products, Customers, and Loyalty Points are created and tested here before moving to production. |
|                                                                                                    |
| Sandbox Usage                                                                                      |
| Sandboxes (Developer, Partial, or Full) replicate the production environment for testing.          |
| For example, a Full Sandbox is used to test seasonal sale workflows and campaign automation without affecting live customers. |
|                                                                                                    |
| Deployment Basics                                                                                  |
| Deployment in Salesforce can be done using Change Sets, Salesforce CLI, or third-party DevOps tools. |
| For the e-commerce CRM, customizations such as objects, workflows, and security settings are deployed from Sandbox → Production using Change Sets. |
|                                                                                                    |
+----------------------------------------------------------------------------------------------------+
```
