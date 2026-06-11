<div align="center">

<img src="https://img.shields.io/badge/Platform-Webflow%20CMS-4353FF?style=for-the-badge&logo=webflow&logoColor=white" />
<img src="https://img.shields.io/badge/Type-Smart%20Onboarding%20Form-E84E0F?style=for-the-badge" />
<img src="https://img.shields.io/badge/Steps-4%20Steps-28A745?style=for-the-badge" />
<img src="https://img.shields.io/badge/Time-~2%20Minutes-FFC107?style=for-the-badge" />
<img src="https://img.shields.io/badge/License-MIT-6C757D?style=for-the-badge" />

<br/><br/>

# 🧑‍💼 Smart Onboarding Form

### A polished, multi-step user profile onboarding form — built with **Webflow CMS**

*Progressive data collection · Real-time auto-save · Animated progress tracking*

</div>

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Live Preview](#-live-preview)
- [Features](#-features)
- [Form Steps](#-form-steps-breakdown)
- [Progress Logic](#-progress-tracker-logic)
- [Design System](#-design-system)
- [Color Palette](#-color-palette)
- [Typography](#-typography)
- [Component Anatomy](#-component-anatomy)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Webflow CMS Setup](#-webflow-cms-setup)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🧭 Overview

**Smart Onboarding Form** is a fully functional, visually polished **4-step user profile form** built on the **Webflow CMS platform**. It's designed to guide new users through a seamless onboarding experience — collecting personal, address, education, and resume information — with live progress tracking, step validation, and auto-saving functionality.

> 🔖 *"Smart onboarding · 4 steps · ~2 min"*

This project demonstrates best-in-class UX patterns for onboarding flows, combining Webflow's visual builder, CMS collections, and Interactions for a no-code production-ready solution.

---

## 🔗 Live Preview

| Resource | Link |
|----------|------|
| 🌐 Live Site | [https://mutli-step-form-cms.webflow.io/](#) |
| 🧩 Webflow Clone | [Clone on Webflow](#) |
| 💻 GitHub Repo | [github.com/busrulnakibbahid/cms-multi-step-form](#) |

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔢 **4-Step Form Flow** | Breaks profile setup into 4 focused, digestible steps |
| 📊 **Live Progress Bar** | Orange animated bar fills from 0% → 100% across steps |
| ✅ **Step Completion Indicators** | Green checkmark icons appear on each completed step node |
| 💾 **Auto-Save on Type** | Form data is saved in real-time — no data lost on navigation |
| 🔒 **Smart Validation** | Next button stays disabled until all required fields are filled |
| 🔁 **Back / Next Navigation** | Full step-by-step navigation with animated transitions |
| 📋 **Dynamic Section Headers** | Each step has a labeled orange banner ("Step 01", "Step 02"...) |
| 🏁 **Submit on Final Step** | Green "Submit" button appears only at Step 4 |
| 📱 **Fully Responsive** | Adapts from mobile to widescreen without breaking layout |
| 🎨 **Custom Branded UI** | Signature orange/green palette with a clean card-based layout |

---

## 📋 Form Steps Breakdown

### ▶ Step 01 — Personal Information
> Progress: **0%** | Status indicator: 🟠 Active

Collects the user's fundamental identity details.

```
┌────────────────────────────────────────────────┐
│  👤  Full Name         → Text Input             │
│  ✉️  Email Address     → Email Input            │
│  📞  Phone Number      → Tel Input              │
│  ⚥   Gender           → Dropdown Select        │
└────────────────────────────────────────────────┘
```

| Field | Input Type | Placeholder | Required |
|-------|-----------|-------------|----------|
| Full Name | `text` | *Enter Your Name....* | ✅ Yes |
| Email Address | `email` | *Enter Your Email....* | ✅ Yes |
| Phone | `tel` | *Enter Your Phone....* | ✅ Yes |
| Gender | `select` | *Select one...* | ✅ Yes |

---

### ▶ Step 02 — Address Information
> Progress: **29%** | Status indicator: 🟠 Active | Step 1: ✅ Completed

Collects the user's physical location details.

```
┌────────────────────────────────────────────────┐
│  📍  Street Address    → Text Input (full width)│
│  🏙️  City              → Text Input (half)      │
│  🏔️  State / Region   → Text Input (half)      │
│  #   Zip / Postal Code → Text Input (half)      │
│  🌍  Country           → Dropdown Select (half) │
└────────────────────────────────────────────────┘
```

| Field | Input Type | Placeholder | Required |
|-------|-----------|-------------|----------|
| Street Address | `text` | *Enter Your Address....* | ✅ Yes |
| City | `text` | *Enter Your City....* | ✅ Yes |
| State / Region | `text` | *Enter Your State....* | ✅ Yes |
| Zip / Postal Code | `text` | *ZIP/Postal Code....* | ✅ Yes |
| Country | `select` | *Select one...* | ✅ Yes |

---

### ▶ Step 03 — Education Information
> Progress: **64%** | Status indicator: 🟠 Active | Steps 1–2: ✅ Completed

Collects academic background and qualifications.

```
┌────────────────────────────────────────────────┐
│  🏛️  Institution Name  → Text Input (full width)│
│  🎓  Degree            → Dropdown Select (half) │
│  📚  Field of Study    → Text Input (half)      │
│  📅  Graduation Year   → Number Input (full)    │
└────────────────────────────────────────────────┘
```

| Field | Input Type | Placeholder | Required |
|-------|-----------|-------------|----------|
| Institution Name | `text` | *Enter Your Institution Name....* | ✅ Yes |
| Degree | `select` | *Select one...* | ✅ Yes |
| Field of Study | `text` | *Enter Your Study Field....* | ✅ Yes |
| Graduation Year | `number` | *Graduation Year....* | ✅ Yes |

---

### ▶ Step 04 — Resume Information
> Progress: **100%** | Status indicator: 🟠 Active | Steps 1–3: ✅ Completed

Final step — collects the user's professional CV/resume link.

```
┌────────────────────────────────────────────────┐
│  📄  CV / Resume URL   → URL Input (full width) │
│                          e.g. https://...       │
└────────────────────────────────────────────────┘
```

| Field | Input Type | Placeholder | Required |
|-------|-----------|-------------|----------|
| CV / Resume Link | `url` | *https://www.facebook.com/* | ✅ Yes |

---

## 📊 Progress Tracker Logic

The progress bar and step indicators update dynamically as the user moves through the form.

```
Step 1 ──────────────── Step 2 ──────────────── Step 3 ──────────────── Step 4
  🟠                      ○                        ○                       ○
  0%                     29%                      64%                    100%
```

| Current Step | Steps Completed | Progress Bar | Percentage |
|-------------|----------------|--------------|------------|
| Step 1 of 4 | None | ░░░░░░░░░░░░░░░░░ | `0%` |
| Step 2 of 4 | Step 1 ✅ | ████░░░░░░░░░░░░░ | `29%` |
| Step 3 of 4 | Steps 1–2 ✅ | ██████████░░░░░░░ | `64%` |
| Step 4 of 4 | Steps 1–3 ✅ | █████████████████ | `100%` |

**State visual legend:**
- 🟠 `Orange circle with number` → Current active step
- ✅ `Green circle with checkmark` → Completed step
- ⚪ `Gray circle with number` → Upcoming step

---

## 🎨 Design System

### Color Palette

The entire UI is built around a warm, energetic palette anchored by a signature orange-red as the primary action color.

---

#### 🔴 Primary — Action Orange
Used for: CTA buttons, step banners, active step indicators, progress bar, icons

| Name | Hex | Usage | Swatch |
|------|-----|-------|--------|
| Primary Orange | `#E84E0F` | Main CTA, Step banners, Active step | ![#E84E0F](https://img.shields.io/badge/-%23E84E0F-E84E0F?style=flat-square) |
| Orange Dark | `#C43A08` | Hover state on primary buttons | ![#C43A08](https://img.shields.io/badge/-%23C43A08-C43A08?style=flat-square) |
| Orange Light | `#F3855C` | Icon fills, secondary highlights | ![#F3855C](https://img.shields.io/badge/-%23F3855C-F3855C?style=flat-square) |
| Orange Pale | `#FAEADA` | Soft background tints | ![#FAEADA](https://img.shields.io/badge/-%23FAEADA-FAEADA?style=flat-square) |

---

#### 🟢 Success — Completion Green
Used for: Completed step checkmarks, Submit button, validation success

| Name | Hex | Usage | Swatch |
|------|-----|-------|--------|
| Success Green | `#28A745` | Submit button, Completed step circles | ![#28A745](https://img.shields.io/badge/-%2328A745-28A745?style=flat-square) |
| Green Dark | `#1E7E34` | Submit button hover state | ![#1E7E34](https://img.shields.io/badge/-%231E7E34-1E7E34?style=flat-square) |
| Green Light | `#5CBF6A` | Checkmark icon fill | ![#5CBF6A](https://img.shields.io/badge/-%235CBF6A-5CBF6A?style=flat-square) |
| Green Pale | `#EAF3DE` | Success background tint | ![#EAF3DE](https://img.shields.io/badge/-%23EAF3DE-EAF3DE?style=flat-square) |

---

#### 🔴 Danger — Back Button Red
Used for: Back button background

| Name | Hex | Usage | Swatch |
|------|-----|-------|--------|
| Danger Red | `#DC3545` | Back button background | ![#DC3545](https://img.shields.io/badge/-%23DC3545-DC3545?style=flat-square) |
| Red Dark | `#B02A37` | Back button hover state | ![#B02A37](https://img.shields.io/badge/-%23B02A37-B02A37?style=flat-square) |

---

#### 🔵 Next Button — Disabled State
Used for: Next button when form fields are incomplete

| Name | Hex | Usage | Swatch |
|------|-----|-------|--------|
| Muted Peach | `#F4A98A` | Disabled "Next Button" fill | ![#F4A98A](https://img.shields.io/badge/-%23F4A98A-F4A98A?style=flat-square) |
| Disabled Text | `#FFFFFF` | Text on disabled button | ![#FFFFFF](https://img.shields.io/badge/-%23FFFFFF-white?style=flat-square&labelColor=999) |

---

#### ⬜ Neutral — Background & Surfaces

| Name | Hex | Usage | Swatch |
|------|-----|-------|--------|
| Page Background | `#F5F0EB` | Warm off-white page bg | ![#F5F0EB](https://img.shields.io/badge/-%23F5F0EB-F5F0EB?style=flat-square&labelColor=999) |
| Card Surface | `#FFFFFF` | Form card, step card bg | ![#FFFFFF](https://img.shields.io/badge/-%23FFFFFF-white?style=flat-square&labelColor=ccc) |
| Input Border | `#CCCCCC` | Text input borders | ![#CCCCCC](https://img.shields.io/badge/-%23CCCCCC-CCCCCC?style=flat-square) |
| Input Fill | `#FAFAFA` | Input field background | ![#FAFAFA](https://img.shields.io/badge/-%23FAFAFA-FAFAFA?style=flat-square&labelColor=ccc) |
| Step Inactive | `#AAAAAA` | Inactive step number circles | ![#AAAAAA](https://img.shields.io/badge/-%23AAAAAA-AAAAAA?style=flat-square) |
| Progress Track | `#E0D8D0` | Progress bar background track | ![#E0D8D0](https://img.shields.io/badge/-%23E0D8D0-E0D8D0?style=flat-square) |

---

#### ✏️ Typography Colors

| Name | Hex | Usage | Swatch |
|------|-----|-------|--------|
| Heading Black | `#1A1A1A` | Main title "Let's Get To Know You" | ![#1A1A1A](https://img.shields.io/badge/-%231A1A1A-1A1A1A?style=flat-square) |
| Body Dark | `#2D2D2D` | Section titles (e.g. "Personal Information") | ![#2D2D2D](https://img.shields.io/badge/-%232D2D2D-2D2D2D?style=flat-square) |
| Body Muted | `#666666` | Subtitle description text | ![#666666](https://img.shields.io/badge/-%23666666-666666?style=flat-square) |
| Placeholder | `#AAAAAA` | Input placeholder text | ![#AAAAAA](https://img.shields.io/badge/-%23AAAAAA-AAAAAA?style=flat-square) |
| Step Label | `#E84E0F` | "STEP X OF 4" label text | ![#E84E0F](https://img.shields.io/badge/-%23E84E0F-E84E0F?style=flat-square) |
| Button White | `#FFFFFF` | Text on all colored buttons | ![#FFFFFF](https://img.shields.io/badge/-%23FFFFFF-white?style=flat-square&labelColor=999) |

---

### Typography

| Element | Font | Size | Weight | Color |
|---------|------|------|--------|-------|
| Page Title | System / Sans-Serif | `42px` | `700 Bold` | `#1A1A1A` |
| Page Subtitle | System / Sans-Serif | `15px` | `400 Regular` | `#666666` |
| Step Banner Text | System / Sans-Serif | `20px` | `700 Bold` | `#FFFFFF` |
| Section Title | System / Sans-Serif | `20px` | `700 Bold` | `#2D2D2D` |
| Field Label | System / Sans-Serif | `14px` | `500 Medium` | `#2D2D2D` |
| Input Text | System / Sans-Serif | `15px` | `400 Regular` | `#1A1A1A` |
| Placeholder | System / Sans-Serif | `14px` | `400 Regular` | `#AAAAAA` |
| Step Label | System / Sans-Serif | `12px` | `700 Bold` | `#E84E0F` |
| Progress % | System / Sans-Serif | `16px` | `600 SemiBold` | `#1A1A1A` |
| Button Text | System / Sans-Serif | `16px` | `700 Bold` | `#FFFFFF` |
| Badge Text | System / Sans-Serif | `13px` | `500 Medium` | `#444444` |

---

### Spacing & Layout

| Token | Value | Usage |
|-------|-------|-------|
| Page Max Width | `900px` | Centered container |
| Card Padding | `32px 40px` | Inner form card |
| Field Gap | `20px` | Between form fields |
| Section Gap | `32px` | Between form sections |
| Input Height | `48px` | All text inputs |
| Button Height | `52px` | CTA buttons |
| Button Padding | `16px 32px` | Horizontal button padding |
| Border Radius | `8px` | Cards, inputs, buttons |
| Progress Bar Height | `6px` | Progress track bar |

---

## 🧩 Component Anatomy

### Step Indicator Node
```
┌──────────────────────────────────────────────────────────┐
│                                                          │
│   ● ──────────────── ● ──────────────── ● ──── ●        │
│  (1)                (2)                (3)   (4)         │
│   ↑                  ↑                  ↑     ↑          │
│ Orange             Green             Green  Gray         │
│ Active           Completed         Completed Upcoming    │
│                                                          │
│ Progress: ██████████████████░░░░░░░░░░░░░░░   64%       │
│           [──────── Orange Fill ────────]                │
└──────────────────────────────────────────────────────────┘
```

### Form Card
```
┌────────────────────────────────────────────────────┐
│  ██████████████████████████████████████████████  │ ← Orange step banner
│              Step 02                             │
│                                                    │
│  Section Title                                     │
│                                                    │
│  🔶 Field Label                                    │
│  ┌──────────────────────────────────────────────┐ │
│  │  Placeholder text...                         │ │ ← Input field
│  └──────────────────────────────────────────────┘ │
│                                                    │
│  🔶 Field A     🔶 Field B                        │
│  ┌──────────┐   ┌──────────────────────────────┐ │
│  │ Input... │   │ Input...                      │ │ ← 2-col layout
│  └──────────┘   └──────────────────────────────┘ │
└────────────────────────────────────────────────────┘
```

### Navigation Buttons
```
┌─────────────────────────────────────────────────────┐
│                                                     │
│  ┌────────────────┐           ┌───────────────────┐ │
│  │  ← Back Button │           │  Next Button →    │ │
│  │  bg: #DC3545   │           │  bg: #E84E0F      │ │
│  │  (Red / Danger)│           │  or #28A745 Submit│ │
│  └────────────────┘           └───────────────────┘ │
│                                                     │
└─────────────────────────────────────────────────────┘
```

---

## 📁 Project Structure

```
smart-onboarding-webflow/
│
├── 📄 README.md                     # Project documentation (this file)
│
├── 🌐 index.html                    # Exported Webflow HTML
│
├── 🎨 css/
│   ├── smart-onboarding.webflow.css  # Webflow-generated styles
│   └── custom-overrides.css          # Custom style overrides
│
├── ⚡ js/
│   ├── webflow.js                    # Webflow runtime & interactions
│   └── form-steps.js                 # Step logic & progress tracking
│
└── 🖼️ images/
    └── screenshots/
        ├── step-01-personal.png
        ├── step-02-address.png
        ├── step-03-education.png
        └── step-04-resume.png
```

> **⚠️ Note:** This is a **Webflow CMS project**. The Webflow Designer is the primary source of truth. Exported code is for reference and hosting purposes only. Edits should be made inside Webflow.

---

## 🚀 Getting Started

### Option A — View Live
Visit the published Webflow site at: **[https://mutli-step-form-cms.webflow.io/](#)**

### Option B — Clone in Webflow
1. Open the [Webflow Cloneable Link](#)
2. Click **"Open in Webflow"**
3. Customize the CMS collections, styles, and interactions
4. Publish to your own Webflow domain or custom domain

### Option C — Use Exported Code
```bash
# 1. Clone this repository
git clone https://github.com/your-username/smart-onboarding-webflow.git

# 2. Navigate into the project
cd smart-onboarding-webflow

# 3. Open in browser
open index.html

# Or serve locally with any static server:
npx serve .
```

---

## 🗄️ Webflow CMS Setup

This project utilizes **Webflow CMS** for dynamic data handling. Below is the CMS collection schema.

### CMS Collection: `User Profiles`

| Field Name | Field Type | Notes |
|------------|-----------|-------|
| `full-name` | Plain Text | Step 1 |
| `email` | Email | Step 1 |
| `phone` | Phone | Step 1 |
| `gender` | Option | Step 1 |
| `street-address` | Plain Text | Step 2 |
| `city` | Plain Text | Step 2 |
| `state-region` | Plain Text | Step 2 |
| `zip-code` | Plain Text | Step 2 |
| `country` | Option | Step 2 |
| `institution-name` | Plain Text | Step 3 |
| `degree` | Option | Step 3 |
| `field-of-study` | Plain Text | Step 3 |
| `graduation-year` | Number | Step 3 |
| `resume-url` | Link | Step 4 |
| `created-at` | Date/Time | Auto |
| `form-completed` | Switch (Bool) | Auto on submit |

---

## 🤝 Contributing

Contributions, improvements, and forks are welcome!

```
1. 🍴 Fork this repository
2. 🌿 Create your branch:    git checkout -b feature/your-feature-name
3. 💾 Commit your changes:   git commit -m "feat: add your feature"
4. 📤 Push to branch:        git push origin feature/your-feature-name
5. 🔃 Open a Pull Request
```

Please follow [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.

---

## 📜 License

This project is licensed under the **MIT License**.

```
MIT License — Copyright (c) 2026 Nusrul Nakib Nahid

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files, to deal in the Software
without restriction — including the rights to use, copy, modify, merge,
publish, distribute, sublicense, and/or sell copies.
```

See the full [LICENSE](./LICENSE) file for details.

---

## 👤 Author

**Name**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/nakib-nahid)

---

<div align="center">

### ⭐ If this project helped you, please give it a star!

*It helps others discover this project and motivates further development.*

<br/>

> 🔖 Built with ❤️ on **Webflow CMS** — *Smart onboarding · 4 steps · ~2 min*

</div>
