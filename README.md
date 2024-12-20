# MINA Protocol Navigators Season 2: Growth Grants Proposal

## Title: 
ZkScholar

## Proposal Overview:

### Problem:
Each year, over $250 billion in financial aid is distributed to students through outdated, inefficient, and insecure systems. These traditional processes are:
- **Cumbersome**: Students must repeatedly submit sensitive personal and financial information to multiple institutions, creating frustration and unnecessary complexity.
- **Insecure**: Centralized databases storing sensitive data are highly vulnerable to breaches, exposing students to identity theft and privacy violations.
- **Slow and Unreliable**: Determining aid eligibility often takes weeks or months, while fund disbursements are delayed, leaving students unable to manage their finances, pay tuition, or continue their education without disruption.
These systemic inefficiencies lead to increased administrative burdens, data privacy concerns, and student financial instability.

### Solution:
ZkScholar introduces a revolutionary approach to financial aid distribution: a streamlined, secure, and private platform that leverages blockchain technology and zk-SNARKs (zero-knowledge proofs) to eliminate inefficiencies while crucially preserving privacy. Below are several of ZkScholar’s unique value propositions:
- **Privacy-Preserving Submissions**: Students can prove financial need without revealing sensitive personal or financial data. Instead of exposing raw information, zero-knowledge proofs validate eligibility privately and securely.
- **Transparent Yet Anonymous Verification**: Colleges set financial aid criteria through a simple user interface. The platform matches eligible students to aid options while ensuring only anonymized eligibility results are visible to institutions.
- **Real-Time Feedback**: Students receive immediate, transparent feedback on their aid eligibility, reducing uncertainty and accelerating decision-making.
By replacing outdated systems with a fully on-chain, privacy-first platform, ZkScholar solves the core issues of insecurity, inefficiency, and delays in financial aid. Therefore, ZkScholar has the potential to be a transformative solution to a decades-old problem.

### Impact:
ZkScholar offers a private, efficient, and verifiable alternative for students seeking financial aid and providers looking to ensure resources are allocated to those truly in need. By leveraging Mina's zk-SNARK technology, the solution eliminates the need to expose sensitive personal and financial data, creating a system that is both secure and equitable.

The proposal encourages adoption on two fronts: students and financial aid providers. For students, it lowers barriers to applying for aid by offering privacy and efficiency, fostering trust in the platform. For providers, it ensures a streamlined, reliable, and provably fair distribution system, increasing confidence in their processes. This dual benefit brings new users into the Mina ecosystem and demonstrates its potential as a robust infrastructure for sensitive, trust-driven applications.

Beyond onboarding users, the proposal serves as a compelling example of Mina’s utility, attracting developers and innovators to explore similar use cases. Showcasing how zk-SNARKs can solve tangible problems in a scalable and decentralized manner paves the way for novel applications in areas like identity verification, private transactions, and secure data sharing.

### Target Audience:
Students who require financial aid, and financial aid providers (benefactors, universities/other educational instituitions, charities, government)

## Architecture & Design:
### Technical Design Overview: 
**1. Frontend (User Interface):**
- Tech Stack: React.js / Next.js, and TypeScript for building an interactive, responsive, and user-friendly interface.
- Features:
  - Web2-friendly authentication via email login for students and financial aid providers (integrating solutions like Web3Auth).
  - Dynamic dashboards for students to apply for aid and for providers to manage aid options.
  - Real-time feedback on aid eligibility based on zk-SNARK verification results.
- Design Tools: Figma for UI/UX design.

**2. Backend:**
- Tech Stack: C# .NET/Golang for API management and business logic.
- Database: PostgreSQL for storing non-sensitive metadata related to aid options and user interactions.
- Role:
  - Managing CRUD operations for financial aid data created by institutions or benefactors.
  - Orchestrating the communication between the frontend, blockchain, and off-chain verification processes.
    
**3. Smart Contracts (On-Chain Logic):**
- Blockchain: Built on Mina Protocol to leverage zk-SNARK technology for privacy-preserving proofs.
- Components:
  - Aid Eligibility Verification Contract: Smart contracts validate student eligibility via zk-SNARKs without exposing sensitive personal or financial information.
  - Aid Fund Release Contract: Automates disbursement of funds to eligible students when criteria are met.
- Interactions:
  - Students submit zero-knowledge proofs proving eligibility.
  - Institutions interact with on-chain contracts to set criteria and verify aid requests.
    
**4. Zero-Knowledge Proof Integration:**
- Role: zk-SNARKs ensure eligibility verification occurs privately without revealing sensitive inputs (e.g., income or personal data).
- Process Flow:
  - Students generate zk-proofs locally and submit them to the Mina blockchain for verification.
  - Institutions only receive proof verification results (e.g., eligible/ineligible) rather than raw student data.
 
## Architecture & Design
### Design Flow:
- **Financial Aid Provider Workflow**
  - Login → Create and manage aid opportunities (criteria, amount, deadlines) → Deploy eligibility logic on-chain → Review anonymous proof submissions.
- **Student Workflow**
  - Login → View available aid options → Submit zk-proof to prove eligibility → Receive instant verification feedback → Approved applications trigger automated aid release.
 
### Vision
We want to first provide a private, trustworthy, and efficient platform where financial aid can be distributed fairly. Our long-term vision is for our platform to eventually become the go-to-platform for effective distribution of funds (e.g. charities, government subsidies, payrolls)

### Production Timeline
The platform will be built and delivered over a 3-month development cycle with clear milestones:
1. **Month 1: Initial Development & Architecture Setup**
  - Design landing page and frontend mockups.
  - Develop backend API with CRUD operations.
  - Set up Web2-friendly logins that with wallet abstraction.
  - Design and create smart contracts for financial aid eligibility verification.
2. **Month 2: Integration & Core Features**
  - Integrate smart contracts with the frontend and backend.
  - Implement zero-knowledge proof generation and verification mechanisms.
  - Complete the student/provider dashboards.
3. **Month 3: Beta Testing & Deployment**
  - Conduct beta testing with local students and financial aid providers.
  - Gather user feedback and optimize for UX.
  - Deploy a production-ready platform with all core functionalities.

## Budget & Milestones
### Deliverables:
- Completed Landing Page for ZkScholar
- Email (Web2-friendly) login for students and financial aid providers on platform
- Well-designed frontend that students and providers will interact with
- CRUD operations on financial aid options by providers
- Automated release of test funds when financial aid is approved
- Beta tested with local students
- Fully deployed web app available for providers and students to start using the platform

### Mid-point Milestones:
- Completed landing page
- Deployed smart contracts for storing and verifying student information
- Integrate frontend to correctly call smart contract and verify student’s eligibility for financial aid

### Project Timeline: 
3 Months

### Budget Requested: 
50,000 MINA

### Budget Breakdown: 
- 4,000 MINA Monthly Stipend Per Team Member, over 3 Months: 4,500 x 3 x 3 = 40,500 MINA
- Marketing: 4,000 MINA
- Server and Database hosting: 1,500 MINA
- Miscellaneous Costs (Pilot programmes, outreach): 4,000 MINA

### MINA Wallet Address:
B62qqq2MwRkjwRCAMF7D7SKsJaWLegc6ZUH5JavycHgq1tg9iMWA1py

## Team Info:
### Proposer Github:
Sean: https://github.com/seanmanik

Joshua: https://github.com/joshuan98 

### Team Members & Experience:
#### 1. Sean Spencer Manik

**Role**: Blockchain Developer

**Github Profile:** https://github.com/seanmanik

**Relevant Experience:**
- Blockchain Engineer at Genesis Block - built collateralized loan platform on EVM chains
- Backend Engineer Intern at Jupiter Exchange 
- Developed DocuEarn at ETHGlobal Bangkok, developing…. Awarded Best Use of WorldID by Worldcoin (3rd). 
- Developed RentGuard at HackRU by Rutgers University, developing smart contracts in Cairo and deploying to Starknet's testnet to facilitate rent hike control and rent collection. Awarded Best Use Of Starknet prize for delivering the top project utilizing the Starknet blockchain.
- Developed DeFi Fraud at TartanHacks by Carnegie Mellon University in Pittsburgh, by creating smart contracts on the XRP Ledger to ensure the legitimate use of government grants. Awarded the XRP Ledger Ripple Prize for delivering the top project utilizing the XRP Ledger.
- Developed TrustTrace at HackHarvard in Cambridge, Massachusetts, by utilizing smart contracts to establish a trustless fundraising system that inspires donor confidence for humanitarian aid initiatives. Awarded 3rd Overall Best Hack out of 600+ participants.
- Developed Connectify, Radiance, and Trailblazer at NEAR Hack-o-Ween in New York, deploying smart contracts on the NEAR Protocol's blockchain:
  - Connectify (1st Place for LLM Model Governance): Stored New York City residents' feedback on-chain and enabled policy generation to improve NYC using blockchain-backed data retrieval.
  - Trailblazer (1st Place for Green Ghouls UrbanTech): Built a Google Maps alternative that rewards sustainable practices with tokens on NEAR. Implemented an on-chain messaging and point tracking system.
  - Radiance (2nd Place for The Scary Black Button): Created a platform that lets users read and leave positive messages on the blockchain, giving purpose to a simple black button.

#### 2. Joshua Nee Ting Feng 

**Role**: Front-end Engineer

**Github Profile:** https://github.com/joshuan98

**Relevant Experience:**
- Front-end Engineer for DocuEarn (at ETHGlobal Bangkok), a privacy-focused dApp enabling passive income from health data using zero-knowledge proofs. Implemented Web3Auth for seamless user onboarding and leveraged TypeScript, React, and Vite for a polished user interface. Achieved runner-up in Polygon’s Real-World Impact: Best Social Good Application track.
- Front-end Engineer for ZkScholar (at ETHGlobal Singapore), a decentralized application streamlining private financial aid applications with zk-SNARKs. Built the Next.js and TypeScript frontend, integrated World ID for secure authentication. Awarded 3rd place among 309 projects in Worldcoin’s Best Use of World ID track.
- Front-end Engineer for ArcAid (at PennApps XXIV by University of Pennsylvania), a zk-SNARK-enhanced student aid application platform. Employed Next.js, Prisma, PlanetScale, and SHA256 encryption to deliver a secure, user-friendly interface. Earned the Best Education Hack award, placing top 8 out of 354 participants.
- Full-stack Engineer for TravelGPT (at HawkHack 2023 by Montclair State University), a customizable travel itinerary generator utilizing OpenAI models and MapBox. Integrated interactive map features and responsive UI elements, securing 1st Place Best Solo Hack.
- Full-stack Engineer at the Singapore Blockchain Innovation Challenge, implementing a web application enabling instant insurance payouts through blockchain interoperability. Leveraged the Affinidi platform for certificate verification and deployed on ZKSync’s Layer-2 to reduce gas costs, winning 3rd Place in the Enthusiast Track.
- Full-stack Software Engineer at InTune Auto (New York), delivering 9 major frontend projects to streamline user workflows including authorization, reminders, scheduling, and integration with Twilio SMS/Gmail. Overhauled Cypress tests to achieve over 90% coverage, utilized TypeScript, React, and Dockerized deployments on AWS ECS, and integrated OpenAI to enhance user experience.
- Software Engineer at ST Engineering (Singapore), developing 11 XR frontends in Swift and VisionOS for Apple Vision Pro. Unified multiple application capabilities into coherent workflows and established strategic foundations for future AR/VR integrations.

#### 3. Beverly Wan Jie Yi

**Role**: Product Manager & Designer

**Relevant Experience:**
- Product Designer for DocuEarn (at ETHGlobal in Bangkok), a privacy-focused dApp that allows anybody to earn USD by contributing confidential health data to research studies, without compromising their privacy. Awarded Best Use of WorldID by Worldcoin (3rd). 
- Product Manager at Inspire Labs (New York), leading a cross-functional team of 8 developers and a UI/UX designer to complete the end-to-end product development of multiple features within the Inspire HUB marketplace, increasing Daily Active Users (DAU) by 30% and registrations by 25%. Created product roadmaps, defined tasks for upcoming sprints, and wrote detailed user stories to explain business logic to the technical team, accelerating time from feature conception to launch by 33%.
- Product Designer for DeFi Fraud (at Tartan Hacks by Carnegie Mellon University), a proactive solution for enforcing compliant grant expenditure on only pre-approved contractors by distributing grants through smart contracts. Won XRP Ledger Ripple Prize for delivering the top project utilizing the XRP Ledger in the On-chain Finance Challenge. 
- Product Designer for RENEW Jersey (at HackTCNJ by The College of New Jersey), a community-based equity crowdfunding platform for urban renewal & redevelopment through the utilization of smart contracts to deploy invested funds. Won Best Front-end Design.
- Product Designer for Trailblazer (at NEAR Hack-o-Ween in New York), a Google Maps alternative that rewards sustainable practices with tokens on NEAR, including on-chain messaging and point tracking system. Won 1st Place for Green Ghouls UrbanTech Bounty.

### Team Achievements:
- ETHGlobal Bangkok (DocuEarn): Best Social Good Application on Polygon (Runners-up): https://ethglobal.com/showcase/docuearn-bsggm
- ETHGlobal Singapore (ZkScholar): Best Use of World ID (3rd): https://ethglobal.com/showcase/zkscholar-yiqo9 

## Risks & Mitigations:
### Project Risks:
1. **Resistance to Adoption by Institutions:**
Universities and benefactors may be hesitant to transition to blockchain-based systems for financial aid due to limited understanding of Web3 technologies, zero-knowledge proofs (zk-SNARKs), and decentralized applications.

2. **Lack of User Awareness and Trust:**
Students and institutions may not initially trust or understand the concept of privacy-preserving proofs and how zk-SNARKs can ensure financial aid eligibility securely and privately.

3. **User Onboarding Challenges:**
Transitioning non-technical users, such as students and institutions unfamiliar with blockchain, to use wallets and interact with decentralized apps (dApps) might lead to a steeper learning curve.

### Mitigation Measures:
1. **Education and Training Programs:**
  - Create user guides and videos to educate institutions and benefactors about blockchain technology and zk-SNARKs.
  - Provide demonstrations and pilot programs to showcase the platform's reliability.

2. **Focus on User Experience:**
  - Develop an intuitive, Web2-friendly interface with seamless onboarding processes (e.g., email logins for students and providers).
  - Abstract away blockchain complexities by implementing custodial or third-party wallet integrations like Web3Auth to reduce friction.

3. **Early Pilot Programs:**
  - Partner with a few universities or benefactors to conduct pilot projects. Use feedback to refine the platform and demonstrate proof-of-concept success.
  - Share success stories and case studies to build credibility and encourage broader adoption.


  



