# Manual Testing Project — E-Commerce Web Application

## Overview
This repository contains the complete manual QA documentation for an **e-commerce web application**, covering the full testing lifecycle — planning, test design, execution, defect reporting, and final sign-off. It includes the test plan, test cases, requirements traceability matrix (RTM), 11 detailed bug reports with screenshots, a consolidated bug report spreadsheet, and a final test summary report.

The goal of this project was to manually validate core e-commerce user journeys — browsing, cart, checkout, login, and navigation — and surface real, reproducible defects the way a QA engineer would on a live project.

**Website Tested:** [SauceDemo E-commerce Web Application](https://www.saucedemo.com)

---

## Application Under Test (AUT)
| Detail | Description |
|---|---|
| **Website** | [SauceDemo](https://www.saucedemo.com) |
| **Application Type** | E-commerce web application |
| **Core Modules Tested** | Product catalog, cart, checkout, login, navigation, UI |
| **Testing Type** | Manual — functional, UI, negative, and exploratory testing |
| **Test Levels** | System testing / end-to-end testing |
| **Environment** | Web browser (desktop) |
| **Test Data** | Sample product catalog, test user accounts, sample addresses/payment data |

---

## Objectives
- Validate core shopping flows work as expected (browse → cart → checkout)
- Verify form validation and error handling across checkout fields
- Confirm UI consistency and correct rendering across pages
- Identify and document defects with clear reproduction steps
- Provide full traceability between requirements and test coverage
- Deliver a final quality assessment to support a release decision

---

## Repository Structure

```
├── README.md
├── Test_Plan
├── Test_Cases
├── RTM
├── Test_Summary_Report
├── Bug_Reports.xlsx
├── Bug_Reports/
│   ├── BUG-01_Items_cannot_be_removed_from_cart_problem
│   ├── BUG-02_Checkout_blocked_Last_Name_field_is_not_...
│   ├── BUG-03_Product_images_do_not_match_product_name
│   ├── BUG-04_Checkout_does_not_complete_after_clicking
│   ├── BUG-05_Sorting_inventory_throws_an_application_...
│   ├── BUG-06_About_menu_link_leads_to_a_broken_404_page
│   ├── BUG-07_Checkout_Name_Zip_fields_accept_invalid
│   ├── BUG-08_Checkout_can_be_completed_with_an_empty
│   ├── BUG-09_UI_icons_render_tilted_misaligned_visual
│   ├── BUG-10_No_loading_indicator_during_delayed_login
│   └── BUG-11_Certain_products_cannot_be_added_to_cart
└── Screenshots/
    ├── BUG-01_Items_cannot_be_removed_from_cart_problem.png
    ├── BUG-02_Checkout_blocked_Last_Name_field_is_not_....png
    ├── BUG-03_Product_images_do_not_match_product_name.png
    ├── BUG-04_Checkout_does_not_complete_after_clicking.png
    ├── BUG-05_Sorting_inventory_throws_an_application_....png
    ├── BUG-06_About_menu_link_leads_to_a_broken_404_page.png
    ├── BUG-07_Checkout_Name_Zip_fields_accept_invalid.png
    ├── BUG-08_Checkout_can_be_completed_with_an_empty.png
    ├── BUG-09_UI_icons_render_tilted_misaligned_visual.png
    ├── BUG-10_No_loading_indicator_during_delayed_login.png
    └── BUG-11_Certain_products_cannot_be_added_to_cart.png
```

---

## Contents

| Document | Description |
|---|---|
| [Test_Plan](./Test_Plan) | Scope, approach, resources, entry/exit criteria, and schedule for the testing effort |
| [Test_Cases](./Test_Cases) | Full set of manual test cases executed against the application, covering positive, negative, and boundary scenarios |
| [RTM](./RTM) | Requirements Traceability Matrix mapping requirements to test cases and execution status |
| [Bug_Reports.xlsx](./Bug_Reports.xlsx) | Consolidated spreadsheet log of all 11 bug reports, with columns for Bug ID, Title, Module, Severity, Priority, and Status — useful as a quick-reference defect tracker alongside the individual bug report write-ups |
| [Test_Summary_Report](./Test_Summary_Report) | Final summary of testing results, defect metrics, and overall quality assessment |

---

## Test Execution Summary
| Metric | Result |
|---|---|
| Total Modules Tested | 6 (Catalog, Cart, Checkout, Login, Navigation, UI) |
| Total Test Cases Executed | See [Test_Cases](./Test_Cases) |
| Total Defects Logged | 11 |
| Defect Areas | Cart (2), Checkout (4), Catalog (1), Navigation (1), UI (1), Performance (1), Functionality (1) |
| Reporting Format | Individual bug reports + screenshot evidence per defect, plus a consolidated [Bug_Reports.xlsx](./Bug_Reports.xlsx) tracker |

---

## Bug Reports

| ID | Summary | Module | Type |
|---|---|---|---|
| BUG-01 | Items cannot be removed from cart | Cart | Functional |
| BUG-02 | Checkout blocked — Last Name field validation issue | Checkout | Functional / Validation |
| BUG-03 | Product images do not match product name | Catalog | Data / UI |
| BUG-04 | Checkout does not complete after clicking submit | Checkout | Functional |
| BUG-05 | Sorting inventory throws an application error | Functionality | Functional |
| BUG-06 | About menu link leads to a broken 404 page | Navigation | Functional |
| BUG-07 | Checkout Name/Zip fields accept invalid input | Checkout | Validation |
| BUG-08 | Checkout can be completed with empty required fields | Checkout | Validation |
| BUG-09 | UI icons render tilted / misaligned | UI | Visual |
| BUG-10 | No loading indicator during delayed login | Performance / UX | Usability |
| BUG-11 | Certain products cannot be added to cart | Cart | Functional |

Each bug report follows a consistent format — **Bug ID, Title, Environment, Steps to Reproduce, Expected Result, Actual Result, Severity, Priority, and Screenshot** — and includes a corresponding screenshot in the [`Screenshots/`](./Screenshots) folder for visual evidence. The [Bug_Reports.xlsx](./Bug_Reports.xlsx) spreadsheet consolidates all 11 defects into a single sortable/filterable log for quick review.

---

## Key Observations
- The **checkout module** accounted for the highest number of defects, indicating it was the highest-risk area of the application and a priority for regression testing.
- Several issues were related to **input validation**, suggesting front-end and back-end validation rules were inconsistently enforced.
- One **usability gap** (missing loading indicator) was logged even though it wasn't a functional break, since it directly affects user experience and perceived reliability.

---

## Tools & Techniques Used
- **Manual testing** — exploratory and scripted execution
- **Test design techniques** — equivalence partitioning, boundary value analysis, negative testing
- **Bug tracking** — structured bug report documentation with reproducible steps, consolidated in [Bug_Reports.xlsx](./Bug_Reports.xlsx)
- **Traceability** — RTM linking requirements to test coverage
- **Documentation** — spreadsheet-based test cases, RTM, and reporting

---

## How to Navigate This Repo
1. Start with the [Test_Plan](./Test_Plan) to understand testing scope and strategy
2. Review [Test_Cases](./Test_Cases) and the [RTM](./RTM) for coverage details
3. Open [Bug_Reports.xlsx](./Bug_Reports.xlsx) for a quick, consolidated view of all defects
4. Browse [Bug_Reports/](./Bug_Reports) for detailed defect write-ups
5. Cross-reference each bug with its screenshot in [Screenshots/](./Screenshots)
6. Read the [Test_Summary_Report](./Test_Summary_Report) for the final quality verdict

---

## Author
**Manual QA Tester**
This project was built to demonstrate a complete, professional manual testing process — from planning through execution to final reporting — reflecting the workflow followed on a real QA team.
