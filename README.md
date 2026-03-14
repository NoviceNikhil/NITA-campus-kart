# NITA-campus-kart
This project is about creating an online portal to provide facility of providing multiple campus essentials with comfort and convenience to students
NIT AP Campus Kart

Overview
NIT AP Campus Kart is a robust, full-stack web application designed to revolutionize in-campus commerce at the National Institute of Technology Andhra Pradesh. This platform streamlines online purchases from the canteen and stationery stores, facilitates in‑campus food delivery, enables inter‑student item trading (e.g., exchanging drafters, lab coats, and other essentials from seniors to juniors), supports festival‑specific product sales with dynamic promotions, and even handles health center medicine delivery. Built entirely with vanilla HTML5, CSS3, and JavaScript (ES6+), the app leverages localStorage for seamless data persistence, eliminating the need for a traditional backend server. This frontend‑only architecture ensures instant accessibility, zero server dependency, and lightning‑fast performance, making it ideal for campus‑wide deployment on shared networks.

Key Features & Technical Implementation

Core E‑Commerce & Delivery System
Users can browse, add to cart, and checkout canteen meals, stationery items, festival products, and medicines with simulated real‑time order tracking stored and updated in localStorage. Transactions are handled entirely client‑side through efficient object‑based JavaScript processing, minimizing DOM manipulations and optimizing for fast rendering and smooth state updates.

Built‑in Pseudo Chatbot Service
A frontend‑only pseudo‑chatbot service processes user queries by parsing input strings to detect query types (such as order status, product search, or general support) and returns fixed, context‑aware responses from predefined templates stored in localStorage. This enhances user interaction and support without relying on external APIs or a backend.

Advanced Marketplace for Bartering & Trading
A dedicated peer‑to‑peer marketplace allows students to exchange items like lab coats, drafters, old textbooks, and other essentials between seniors and juniors. Listings include item descriptions, images, barter terms, and a simple messaging interface powered by the pseudo‑chatbot. All data is persisted in localStorage with unique transaction identifiers and structured JavaScript objects.

Dynamic Festival Offers & Promotions
Festival‑specific offers (e.g., Diwali or Holi specials) are showcased in a rotating banner carousel built with CSS animations and JavaScript intervals. The banners slide in and out with easing transitions (using cubic‑bezier timing functions), ensuring smooth, visually engaging promotions that update automatically based on the current date and stored offer schedules.

Custom Animations, Transitions, Popups & Modals
The UI is enhanced with custom CSS keyframe animations, transforms, and backdrop‑filter effects for a polished, dynamic feel. Popups and modals (implemented with position: fixed and CSS Grid/Flexbox) handle carts, order confirmations, and forms, featuring slide‑in/fade effects, drag‑to‑dismiss gestures, and keyboard navigation (e.g., ESC to close) for better accessibility and user control.

Multi‑Role Registration & Authentication
The application provides separate registration and login flows for three user roles:

Students/Users: Standard sign‑up, profile management, and order placement.

Administration (Canteen/Stationery Personnel): Dashboard for store performance analytics, product roster management, dynamic price changes, and creating offers/ads for new products.

Delivery Personnel: Interfaces for viewing assigned orders and updating delivery status.

A forgot password mechanism simulates email recovery using localStorage‑stored timestamps, and passwords are hashed using the crypto.subtle API (or a CryptoJS‑style library) before being stored in localStorage, adding a basic layer of security without a backend.

Performance Optimizations
The codebase follows an object‑oriented, modular JavaScript design with singleton‑style state managers and debounced input handlers to minimize re‑renders and memory usage. Images are lazily loaded where appropriate, and event listeners are carefully cleaned up to avoid leaks. These optimizations ensure fast rendering and smooth interactions even on low‑end devices.

Software Development Life Cycle (SDLC)
The project followed a structured SDLC from inception to deployment:

Information Gathering & Requirement Analysis: Interviews, surveys (over 100 responses), and focus groups with actual canteen/stationery users, service providers, and delivery staff were conducted to uncover pain points such as time wasted traveling from hostels to canteen and the need for easier, more comfortable purchasing and bartering.

Design: High‑fidelity wireframes and UI mockups were created in Figma, emphasizing a responsive, mobile‑first layout built with CSS Grid and Flexbox.

Implementation: The frontend was developed in a modular fashion using JavaScript object patterns, with feature‑based branches managed via Git.

Testing: Basic unit tests and usability tests were carried out with a group of beta users to validate workflows and performance.

Deployment & Maintenance: The application is hosted on GitHub Pages, and project tracking (stories, issues, collaboration) is managed using GitHub Projects to maintain a clear record of tasks, timelines, and memory/time constraints.

Tech Stack

Frontend: HTML5, CSS3 (Grid, Flexbox, animations), JavaScript (ES6+ with localStorage)

State & Persistence: Custom localStorage wrappers with JSON serialization

Security: Client‑side password hashing via crypto.subtle or CryptoJS

UX Enhancements: Custom animations, transitions, modals, and the pseudo‑chatbot

Tools: VS Code, Git, GitHub, GitHub Pages, Figma for UI design
