<div align="center">

# UTKARSH SHIRBHATE

### APPLIED AI · WORKFLOW AUTOMATION · BACKEND ENGINEERING


[![Portfolio](https://img.shields.io/badge/PORTFOLIO-8B5CF6?style=for-the-badge&labelColor=111827)](https://utkarsh-shirbhate-portfolio-website.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LINKEDIN-06B6D4?style=for-the-badge&labelColor=111827)](https://www.linkedin.com/in/utkarshshirbhate)
[![Email](https://img.shields.io/badge/EMAIL-F472B6?style=for-the-badge&labelColor=111827)](mailto:UtkarshShirbhate1311@gmail.com)
[![GitHub](https://img.shields.io/badge/GITHUB-22C55E?style=for-the-badge&labelColor=111827)](https://github.com/Vukung)

</div>

<p align="center">
I build practical software around real operational problems: turning unstructured inputs into useful data, making booking and payment workflows more reliable, and adding the validation and error handling that turns a working demo into a system people can trust.
</p>

<!-- <p align="center">
I'm a 2026 Electronics &amp; Telecommunication Engineering graduate from MIT Academy of Engineering, Pune.<br/>
My work spans LLM-powered automation, backend APIs, full-stack applications, analytics, and focused open-source contributions.
</p> -->

### What I focus on

- Applied AI and workflow automation
- Backend APIs and product workflows
- Reliability, validation, and edge cases

---

## `01 / WHAT I LIKE BUILDING`

- **AI workflows that produce usable data** - schema-constrained classification, output validation, retries, and API-limit handling.
- **Backends with clear rules** - authentication, booking lifecycles, relational data models, payment states, and signed webhooks.
- **Small tools that remove real friction** - from booking interfaces to careful file-system utilities.
- **Software that fails clearly** - useful error messages, testable behaviour, and honest documentation of limitations.

---

## `02 / FLAGSHIP PROJECTS`

### [AI Ad Classification & Decision-Making Workflow](https://github.com/Vukung/AI-Ad-Mapping-Category-Classification-System)
**n8n · Groq / Llama 3.1 · Google Sheets · Looker Studio**

**Why I built it:** During my Business Analyst internship, campaign analysis was slowed down by missing or inconsistent ad classification. Analysts had to inspect ads and manually assign attributes before campaign data could be compared consistently.

This workflow uses an LLM to classify ad copy and campaign fields into structured attributes, then makes the results available for downstream analysis and decision-making. The repository documents handling for API rate limits and failed requests. The project materials report approximately **80% less manual tagging effort**.

**What it demonstrates:** LLM integration, ad classification, structured outputs, workflow orchestration, API reliability, and using classified campaign data to support analysis and decisions.

### [EVE Healthcare API](https://github.com/Vukung/diagnostics-booking-api)
**FastAPI · Pydantic · PostgreSQL · SQLAlchemy · Alembic · JWT · pytest**

**Why I built it:** A diagnostic-test booking API is a good test of whether a backend handles real workflow rules-not just create/read/update/delete endpoints.

The API supports authentication, diagnostic-centre and test listings, user-owned bookings, explicit booking-state transitions, simulated payment attempts, and signed payment webhooks. It stores a price snapshot with each booking, verifies webhook signatures, guards against duplicate webhook events, and applies booking/payment changes transactionally. Automated tests and a separate integration-test database are part of the setup.

**What it demonstrates:** Relational modelling, authorization boundaries, migrations, state machines, webhook verification, idempotency, and testable API design. Payments are simulated for this project; it is not presented as a live payment-provider integration.

### [MyNestor Booking Page](https://github.com/Vukung/mynestor-booking)
**JavaScript · Wix Bookings API · Wix eCommerce API · GitHub Pages**

**Why I built it:** The default booking journey did not offer the required way to show only service providers who cover a customer's postal/PIN code.

The page guides customers through service selection, location filtering, provider selection, available dates and slots, and contact details. It fetches data from Wix and sends customers to Wix-hosted checkout to complete confirmation. That final step matters: creating a booking alone can leave it in an incomplete state until checkout finishes, so the interface follows the platform's actual confirmation behaviour instead of implying that a selected slot is already booked.

**What it demonstrates:** Third-party API integration, client-side workflow design, responsive UI, time-zone handling, and solving a product constraint within an existing platform.

## `03 / MORE PROJECTS & EXPERIMENTS`

The projects below are smaller builds, prototypes, or learning experiments. Expand a section for the context and implementation details.

<details>
<summary><strong>[Resume Rocket](https://github.com/Vukung/Resume-Builder-Webapp)</strong></summary>

**React · Node.js · Express · PostgreSQL / Supabase · JWT**

**Why I built it:** Resume content changes across applications, but maintaining multiple versions should not mean repeatedly rebuilding documents from scratch.

Resume Rocket provides authenticated resume editing, a live preview, and a dashboard to search, duplicate, and soft-delete resume versions. Its editor organises content into reusable sections, backed by an API and relational persistence.

**What it demonstrates:** Full-stack integration, data modelling, authentication, CRUD workflows, and deploying a database-backed application. See the repository for its current setup and demo details.

</details>

<details>
<summary><strong>[Northstar Homes - AI Sales Assistant](https://github.com/Vukung/northstar-homes-ai-agent)</strong></summary>

**Node.js · Express · Groq Llama 3.3 · Vanilla JavaScript**

**Why I built it:** A sales assistant needs more than a convincing conversational tone-it must follow product-specific information and behave sensibly around booking details and user requests.

This take-home prototype gives a fictional real-estate sales consultant a defined persona and project knowledge, with session-aware chat and end-of-session analytics. It includes scripted test cases and guardrails for date-related booking questions. Testing revealed that an opt-out rule enforced through prompting alone was unreliable, so the behaviour needed an implementation-level fix. Sessions are intentionally in memory, and the README documents the prototype's limitations.

**What it demonstrates:** Prompt design, API integration, conversation state, behaviour testing, and recognising when a prompt is not a substitute for application logic.

</details>

<details>
<summary><strong>[Google Takeout JSON Filename Fixer](https://github.com/Vukung/gpth-json-fixer)</strong></summary>

**PowerShell · File-system automation**

**Why I built it:** Google Takeout can export media files and their JSON metadata sidecars with mismatched spaces and underscores. Tools that expect the names to match may miss the sidecar and fail to restore the original media date.

The script recursively checks sidecar filenames, tries underscore/space variants, and renames only JSON sidecars when a matching media file is found. It leaves media untouched and supports a `-DryRun` preview so users can inspect changes before applying them.

**What it demonstrates:** Practical automation, cautious file operations, dry-run safety, and clear documentation of edge cases.

</details>

<details>
<summary><strong>[Personal Portfolio](https://github.com/Vukung/utkarsh-portfolio-website)</strong></summary>

**Next.js · React · TypeScript · Vercel**

My portfolio brings my engineering projects, experience, and credentials into one place. Maintaining it has also involved deployment debugging: tracing a map failure to external tile-provider configuration, improving the fallback behaviour, and keeping resume and certification links current.

</details>

## `04 / OPEN-SOURCE CONTRIBUTIONS`

I contribute to existing codebases as well as building my own projects. These four pull requests were **merged into the upstream [Wallendar project](https://github.com/shm-dtt/wallendar)**; my [account's Wallendar repository](https://github.com/Vukung/wallendar) is a fork, so I link to the upstream PRs to make the contribution trail clear.

- [**AI-powered text overlays and one-liner generation - PR #83**](https://github.com/shm-dtt/wallendar/pull/83): added a 3×3 placement system, multi-line text rendering, Groq-powered mood presets, shared font state, request cancellation, input validation, timeouts, and user-facing error handling.
- [**Past-date strikethrough and today highlighting - PR #91**](https://github.com/shm-dtt/wallendar/pull/91): added calendar-aware rendering, contrast-aware highlighting, opt-in controls, and logic scoped to the current month.
- [**IP-based rate limiting - PR #95**](https://github.com/shm-dtt/wallendar/pull/95): integrated Upstash Redis sliding-window limits (five requests per minute per IP), with a fail-secure production path and a smoother local-development setup.
- [**Google Fonts integration follow-up - PR #109**](https://github.com/shm-dtt/wallendar/pull/109): rebased the feature on the current upstream branch, resolved conflicts, and aligned it with existing project patterns.

I also made focused fixes in other public codebases: a [React/TypeScript runtime and build fix in Reliantai](https://github.com/Getstartified/Reliantai-online/commit/c36fbb29f00fe9a214531f7bd21fef3e52ea6832) and a [navbar logo visibility fix in Docuiq](https://github.com/Getstartified/Docuiq-online/commit/228771c8be1cbd2b565f35a3acf1e7e6f8a58bf9).

## `05 / EXPERIENCE BEHIND THE BUILDS`

<table>
  <thead>
    <tr>
      <th>Organization</th>
      <th>Role</th>
      <th>Duration</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Aristok Technologies</strong></td>
      <td>Business Analyst Intern</td>
      <td align="center">Aug 2025 - Nov 2025</td>
    </tr>
    <tr>
      <td colspan="3">
        <strong>Project Details:</strong>
        <ul>
          <li>Managed analysis for a <strong>₹6 lakh/month performance-marketing budget</strong>.</li>
          <li>Worked with multi-source campaign data, built tracking models and KPI dashboards, and analysed acquisition funnels.</li>
          <li>Resume-reported impact: <strong>28% reduction in cost per acquisition</strong> following spend and audience adjustments.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>PulseOn-EV</strong></td>
      <td>Technical Intern - Web &amp; Mobile Development</td>
      <td align="center">Jun 2025 - Aug 2025</td>
    </tr>
    <tr>
      <td colspan="3">
        <strong>Project Details:</strong>
        <ul>
          <li>Built backend REST APIs for a cross-platform EV service platform handling bookings and authentication.</li>
          <li>Developed secure OAuth and phone-based OTP login, improving usability for older audiences.</li>
          <li>Simplified booking user flows to reduce incorrect service requests by approximately <strong>30%</strong>.</li>
          <li>Integrated Razorpay payments and Google Maps-based real-time tracking for service dispatch.</li>
          <li>Worked in a 3-member team using GitHub for code reviews, pull requests, and conflict resolution.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>Campus Credentials</strong></td>
      <td>Full-Stack Development Intern</td>
      <td align="center">Jun 2024 - Aug 2024</td>
    </tr>
    <tr>
      <td colspan="3">
        <strong>Project Details:</strong>
        <ul>
          <li>Engineered a full-stack blog platform using <strong>React, Node.js, and Express.js</strong>.</li>
          <li>Architected a <strong>MySQL</strong> database with foreign keys and indexing for data integrity.</li>
          <li>Designed a secure RESTful API featuring <strong>JWT and Bcrypt</strong> for user authentication.</li>
          <li>Built an admin dashboard with <strong>Role-Based Access Control (RBAC)</strong> for content moderation.</li>
          <li>Related project: <a href="https://github.com/Vukung/Blog-Website-Project">Blog Website</a>.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>Nekotachi Podcast Community</strong></td>
      <td>Co-founder</td>
      <td align="center">Jan 2023 - Jan 2025</td>
    </tr>
    <tr>
      <td colspan="3">
        <strong>Responsibilities &amp; Impact:</strong>
        <ul>
          <li>Led a 15-member team across content, outreach, and operations.</li>
          <li>Helped deliver 10+ events through planning, structured follow-ups, and team coordination.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


## `06 / PROJECT INDEX`

| Project | What it explores |
| --- | --- |
| [Pune House Price Prediction](https://github.com/Vukung/Pune-House-Price-Prediction) | A small Flask application that serves a trained model for property-price estimates from area and configuration inputs. |
| [Sentiment Analysis from Image Text](https://github.com/Vukung/Sentiment-Analysis-ML-Model) | Extracts text from uploaded images with OCR, cleans the text, and runs sentiment classification. |
| [Driver Distraction Detection](https://github.com/Vukung/-Driver-Distraction-Detection-Using-Deep-Learning) | Team academic project exploring CNN classification across 10 driving-behaviour classes. |
| [Smart Parking System](https://github.com/Vukung/Smart-Parking-System-Using-NodeMCU-IR-Sensors-and-ThingSpeak) | IoT parking occupancy detection using NodeMCU, IR sensors, and ThingSpeak visualisation. |
| [Aerodynamic Motion Classification](https://github.com/Vukung/-Aerodynamic-Motion-Classification-Using-MPU6050-and-STM32) | Embedded sensing with an MPU6050 and STM32, including gyroscope sampling and signal-gradient calculations. |
| [AI Web Automation POC](https://github.com/Vukung/ai-saas-web-automation-poc) | Playwright-based SaaS UI navigation and data extraction, documenting selector brittleness and where semantic/self-healing automation could help. |
| [Andromeda Creative Generator](https://github.com/Vukung/andromeda-creative-generator) | Front-end prototype for planning structurally varied ad creative combinations and flagging possible near-duplicates before export. |
| [SkillGap Finder](https://github.com/Vukung/SkillGap-Finder) | Early browser-based prototype around identifying skills gaps. |
| [Letter Generator - Java](https://github.com/Vukung/Letter-Generator-JAVA-Application) | Early Java application project. |

Some repositories are coursework, prototypes, or experiments rather than production-ready products. I prefer to label them by their actual scope and limitations rather than overstate their maturity.

## `07 / TECH STACK`

**Languages:** Python · JavaScript · TypeScript · SQL · Java · C/C++ · PowerShell  
**AI & data:** LLM APIs · structured prompting · n8n · Pandas · scikit-learn · TensorFlow/Keras · OpenCV · OCR · Looker Studio · Power BI  
**Backend:** FastAPI · Node.js · Express · REST APIs · JWT · webhooks · pytest  
**Frontend:** React · Next.js · HTML · CSS · Tailwind CSS  
**Databases & delivery:** PostgreSQL · MySQL · MongoDB · Git · GitHub · Docker · Vercel · Render · GitHub Pages  
**Embedded & automation:** Playwright · NodeMCU · IR sensors · STM32 · MPU6050 · ThingSpeak

<div align="center">

<img src="https://skillicons.dev/icons?i=python,js,ts,react,nextjs,nodejs,express,fastapi,postgres,mysql,mongodb,git,github,docker,vercel&theme=dark" alt="Technology icons" />

</div>

## `08 / EDUCATION, RESEARCH & CERTIFICATIONS`

### Education

<table>
  <thead>
    <tr>
      <th>Year</th>
      <th>Qualification</th>
      <th>Institution</th>
      <th>Result</th>
      <th>Remark</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">2026</td>
      <td>B.Tech - Electronics and Telecommunication Engineering</td>
      <td>MIT Academy of Engineering, Pune</td>
      <td align="center">8.98/10</td>
      <td>Distinction</td>
    </tr>
    <tr>
      <td align="center">2022</td>
      <td>12th Standard - Maharashtra State Board</td>
      <td>Bhartiya Mahavidyalaya, Amravati</td>
      <td align="center">81%</td>
      <td>Distinction</td>
    </tr>
    <tr>
      <td align="center">2020</td>
      <td>10th Standard - Maharashtra State Board</td>
      <td>Golden Kids English School, Amravati</td>
      <td align="center">85%</td>
      <td>Distinction</td>
    </tr>
  </tbody>
</table>

### Certifications

<table>
  <thead>
    <tr>
      <th>Year</th>
      <th>Certification</th>
      <th>Issuing Organization</th>
      <th>Verification</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">2026</td>
      <td>AWS Certified Cloud Practitioner</td>
      <td>Amazon Web Services (AWS)</td>
      <td><a href="https://www.credly.com/">Credly</a></td>
    </tr>
    <tr>
      <td align="center">2024</td>
      <td>AWS Academy Graduate - Data Engineering</td>
      <td>AWS Academy</td>
      <td><a href="https://www.credly.com/">Credly</a></td>
    </tr>
  </tbody>
</table>

### Research, Publications & Achievements

<table>
  <thead>
    <tr>
      <th>Year</th>
      <th>Category</th>
      <th>Title / Achievement</th>
      <th>Event / Organization</th>
      <th>Contribution / Result</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">2025</td>
      <td>Research Publication</td>
      <td>Sentiment Mining from Social Media Platforms: A Tool for Real-Time Opinion Analysis</td>
      <td>ICTCS 2025</td>
      <td>Co-authored research paper</td>
    </tr>
    <tr>
      <td align="center">2024</td>
      <td>Research Presentation</td>
      <td>Millet Production Management Using Cloud Computing for Farmers</td>
      <td>NCPC 2024, Sinhgad College of Engineering</td>
      <td>Presented research work</td>
    </tr>
    <tr>
      <td align="center">2023</td>
      <td>Competition</td>
      <td>State Rank 17 - Coding Wars</td>
      <td>PCCOE Spectrum</td>
      <td>17th rank</td>
    </tr>
  </tbody>
</table>


---

I’m interested in roles where applied AI, automation, backend systems, and data can make a real workflow more useful and reliable.

---

## `09 / GITHUB TELEMETRY`

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Vukung&show_icons=true&hide_border=true&theme=tokyonight&bg_color=0D1117&title_color=22D3EE&icon_color=A78BFA&text_color=C9D1D9" alt="GitHub stats" />
<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=Vukung&hide_border=true&theme=tokyonight&background=0D1117&ring=A78BFA&fire=F472B6&currStreakLabel=22D3EE" alt="GitHub contribution streak" />

</div>


---

<div align="center">

`Build useful things. Make failure visible. Improve the workflow.`

</div>
