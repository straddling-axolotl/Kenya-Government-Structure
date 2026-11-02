# Structure of the Kenyan Government (Interactive Web Application)

An interactive, responsive single-page web visualization detailing the top-down governance framework of the Republic of Kenya under the **2010 Constitution of Kenya**. 

This application maps out the separation of powers across the **Executive, Legislative, and Judicial** arms of government, highlights the **Devolved County Governments**, and clearly distinguishes **Directly Elected Seats** (where citizens vote during general elections) from appointed/nominated positions.

---

## 🌟 Key Features

* **Top-Down Interactive Governance Tree:** Visual breakdown starting from sovereign power under the Constitution down through national and county levels.
* **Filter by Seat Type:** Toggle dynamically between **Voted Seats Only** (the 6 ballot choices: President, Governor, Senator, Woman Rep, MP, MCA) and **Appointed / Nominated Positions**.
* **Detailed Seat & Role Modals:** Deep dives into each constitutional office—including mandates, term limits, election frequency, and legislative scopes.
* **External Legal & Electoral Resources:** Direct reference links to official resources:
  * [Constitution of Kenya (Kenya Law)](https://kenyalaw.org/akn/ke/act/2010/constitution/eng@2010-09-03)
  * [Independent Electoral and Boundaries Commission (IEBC)](https://www.iebc.or.ke/)
* **Zero Dependencies:** Built purely with single-file vanilla HTML, CSS (Tailwind CDN / FontAwesome), and JavaScript for lightweight execution.

---

## 🏛️ Structure Overview

```text
               ┌─────────────────────────────────────────┐
               │    Constitution of Kenya 2010           │
               │         (Sovereign Power)               │
               └────────────────────┬────────────────────┘
                                    │
       ┌────────────────────────────┼────────────────────────────┐
       │                            │                            │
┌──────┴─────────┐           ┌──────┴─────────┐           ┌──────┴─────────┐
│   EXECUTIVE    │           │  LEGISLATURE   │           │   JUDICIARY    │
├────────────────┤           ├────────────────┤           ├────────────────┤
│ • President*   │           │ Parliament:    │           │ • Chief Justice│
│ • Cabinet      │           │ • National     │           │ • Supreme Court│
│ • Civil        │           │   Assembly*    │           │ • Court of     │
│   Service      │           │ • Senate*      │           │   Appeal       │
└────────────────┘           └────────────────┘           │ • High Court   │
                                                          └────────────────┘
                                    │
                         ┌──────────┴──────────┐
                         │ DEVOLVED GOVERNMENTS│
                         │    (47 Counties)    │
                         ├─────────────────────┤
                         │ • County Executive* │
                         │ • County Assembly*  │
                         └─────────────────────┘
                                (* Contains directly elected seats)
```

---

## 🗳️ Directly Elected Positions Included

The application details all **6 elective posts** filled by citizens during a General Election:

1. **President & Deputy President:** Head of State and Executive arm (National level).
2. **Governor & Deputy Governor:** Chief Executive of the County Government (County level).
3. **County Senator:** Representative of the county in the Senate (Bicameral Parliament).
4. **Member of National Assembly (MP):** Representative of single-member constituencies in Parliament.
5. **County Woman Representative:** Women's representative in the National Assembly (1 per county).
6. **Member of County Assembly (MCA):** Ward representative in the County Assembly.

---

## 🚀 Quick Start / Local Setup

Because the application is built as a self-contained static HTML page, no build step, node modules, or database setup is required.

### Options to Run:

1. **Direct Browser Execution:**
   Clone or download the repository and open `index.html` directly in any web browser:
   ```bash
   git clone https://github.com/your-username/kenya-government-structure.git
   cd kenya-government-structure
   # Open index.html in your browser
   ```

2. **Serve with Python (Optional local server):**
   ```bash
   python3 -m http.server 8000
   ```
   Then navigate to `http://localhost:8000` in your web browser.

---

## 🛠️ Built With

* **HTML5** & **Vanilla JavaScript (ES6+)**
* **Tailwind CSS** (via CDN) – Layout and styling
* **FontAwesome 6** – Vector icons
* **Google Fonts (Inter)** – Typography

---

## 📜 License & Legal References

This project is created for educational and civic information purposes. All references to constitutional articles correspond to the **Constitution of Kenya (2010)** as promulgated on August 27, 2010.

* Legal source texts hosted by [Kenya Law](https://kenyalaw.org).
* Electoral guidelines provided by the [IEBC](https://www.iebc.or.ke/).
