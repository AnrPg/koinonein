# Cosmic Hangout (Koinoneīn)

![CI](https://img.shields.io/badge/ci-passing-brightgreen) ![License](https://img.shields.io/badge/license-MIT-blue)

A next‑gen social media platform inspired by the ancient Greek ethos of κοινωνία, blending shared wonder with collective belonging in a seamless, jank‑free experience.

---

## Table of Contents

1. [Project Vibe](#project-vibe)  
2. [Summary of Core Concept](#summary-of-core-concept)  
3. [What Is Shared Wonder?](#what-is-shared-wonder)  
4. [Ancient Greek Roots of κοινωνία](#ancient-greek-roots-of-κοινωνία)  
5. [Getting Started](#getting-started)  
   - [Prerequisites](#prerequisites)  
   - [Installation](#installation)  
6. [Usage](#usage)  
7. [Folder Structure](#folder-structure)
8. [Contributing](#contributing)  
9. [License](#license)  

---

## Project Vibe

Cosmic Hangout is all about co‑experiencing awe in community. We’re crafting a smooth, responsive feed where every scroll ignites conversations, connections, and collective curiosity—just like gazing at the stars together or co‑creating your town’s future. Welcome to your digital κοινωνία.

---

## Summary of Core Concept

Shared wonder is the collective experience of awe and curiosity, where individuals bond over mutual amazement at something novel, inspiring deeper connections and a sense of unity.

---

## What Is Shared Wonder?

Shared wonder describes the phenomenon when a group of people simultaneously encounters something inspiring or mysterious—be it natural beauty, a creative work, or an intellectual insight—and reacts with collective awe and curiosity, strengthening social bonds through that mutual emotional uplift ([IU Blogs][1], [Colorado Mesa University][2]).

In practice, shared wonder might unfold as a community gazing together at a star‑filled sky, sparking conversations about the cosmos and our place in it, which transforms an individual moment of marvel into a shared, unforgettable memory ([Colorado Mesa University][2]).

Similarly, when civic leaders and residents come together to reimagine their town—pausing to listen, dream, and co‑create—they tap into shared wonder, knitting the community into a more resilient, imaginative whole ([coheringcommunity.com][3]).

At its core, shared wonder is about co‑experiencing the exceptional or sublime, turning isolated feelings of amazement into a communal force that fosters empathy, belonging, and collective inspiration ([natalieeslick.com][4]).

[1]: https://blogs.iu.edu/ecohealth/2025/05/27/finding-humanity-in-the-rainforest/?utm_source=chatgpt.com "Finding Humanity in the Rainforest – Planetary Health in Costa Rica"  
[2]: https://www.coloradomesa.edu/now/2025/04/wonder-makes-the-world-go-round.html?utm_source=chatgpt.com "Wonder Makes the World go Round - Colorado Mesa University"  
[3]: https://www.coheringcommunity.com/post/how-leaders-communities-co-create-a-thriving-future/?utm_source=chatgpt.com "A Liberating Dance of Leaders and Community"  
[4]: https://www.natalieeslick.com/blog/share-your-wonder?utm_source=chatgpt.com "Share your wonder - Natalie Eslick"  

---

## Ancient Greek Roots of κοινωνία

In Greek political thought, κοινωνία (koinōnía) in Aristotle’s Politics denotes any form of sharing in common that culminates in the πόλις as the highest community where citizens jointly pursue the common good ([Wikipedia][5], [neomagazine.com][6]). For Plato and other classical philosophers, κοινωνεῖν (koinonein)—mutual participation—was the very practice that forged the polis’ moral and civic cohesion ([Wikipedia][5], [Christos Yannaras' books][7]). Etymologically rooted in κοινός (koinos), “common,” koinonein emphasizes shared values and mutual contribution at the heart of Greek communal life ([Wikipedia][5], [Greek News Agenda][8]). The polis was conceived not merely as a territory or institution but as a living κίνημα κοινωνίας, an organic fellowship of citizens bound by collective virtue and responsibility ([neomagazine.com][6], [ecosemiotics.com][9]). In this view, koinonein transcended economic alliance to embody the deeper Greek ideals of φιλία (philia) and political solidarity that animated civic existence ([Wikipedia][5], [czasopisma.tnkul.pl][10]). Reflecting this ancient ethos in modern thought, one influential Orthodox philosopher interprets the πόλις as an ontological event of free relational communion—arguing that true political existence emerges from this ecclesial κοινωνία of persons rather than coercive state structures ([Academia][11], [ecosemiotics.com][9]). Thus, the ancient practice of koinonein lives on as the foundational principle of community, reminding us that political life is first and foremost a shared ontological journey.

[5]: https://en.wikipedia.org/wiki/Koinonia?utm_source=chatgpt.com "Koinonia"  
[6]: https://neomagazine.com/2009_05_may/24.html?utm_source=chatgpt.com "Reflecting on a Christos Yannaras lecture - NEO ::magazine"  
[7]: https://yannarasbooks.wordpress.com/wp-content/uploads/2020/09/christos-yannaras_-the-apophatic-horizon-of-ontology-basilio-petra.pdf?utm_source=chatgpt.com "[PDF] Christos Yannaras Basilio Petrà"  
[8]: https://www.greeknewsagenda.gr/andreas-andreopoulos/?utm_source=chatgpt.com "Andreas Andreopoulos on Christian Orthodoxy as an expression of ..."  
[9]: https://ecosemiotics.com/2023/05/23/sobornost-in-the-orthodox-church-and-rights-in-todays-virtual-global-west/?utm_source=chatgpt.com "Sobornost in the Orthodox Church and Rights in Today's Virtual ..."  
[10]: https://czasopisma.tnkul.pl/index.php/rt/article/download/2386/1807/6898?utm_source=chatgpt.com "[PDF] The Ethos of God and Man in the Christos Yannaras' Works"  
[11]: https://www.academia.edu/32674259/The_communo_centric_political_theology_of_Christos_Yiannaras_in_conversation?utm_source=chatgpt.com "The communo-centric political theology of Christos Yannaras in ..."  


## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 16+  
- [Yarn](https://yarnpkg.com/) or npm  
- [Docker](https://www.docker.com/) (for local microservices)  
- [Python](https://www.python.org/) 3.9+ & [conda](https://docs.conda.io/) (for FastAPI ML service)

### Installation

1. **Clone repository**  
   ```bash
   git clone https://github.com/your-org/cosmic-hangout.git
   cd cosmic-hangout
   ```

2. **Install frontend dependencies**  
   ```bash
   cd services/frontend
   yarn install
   ```

3. **Install ML service dependencies**  
   ```bash
   cd ../ml-service
   conda create -n cosmic-ml python=3.9
   conda activate cosmic-ml
   conda install -c conda-forge fastapi uvicorn
   ```

4. **Start all services locally**  
   ```bash
   docker-compose up --build
   ```

---

## Usage

- Frontend: http://localhost:3000  
- ML API: http://localhost:8000/docs  

---

## Folder Structure

* **`services/`**

  * **`frontend/`** – The Next.js app housing your React pages, components, and client logic.

    * `pages/` – Route files that render UI and fetch data.
    * `components/` – Reusable React components (buttons, cards, layouts).
    * `next.config.js` – Next.js config for rewrites, plugins, and build tweaks.
  * **`api-gateway/`** – (Optional) A NestJS “backend-for-frontend” layer that unifies and secures calls to downstream services.
  * **`auth-service/`** – NestJS microservice handling signup, login, JWT issuance, and user authentication logic.

    * `src/controllers/` – REST endpoints for auth flows (login, register, refresh‑token).
    * `src/modules/` – NestJS modules wiring up controllers, services, and providers.
    * `src/services/` – Business logic for password hashing, token generation, and user lookup.
    * `src/main.ts` – Bootstraps the NestJS app.
    * `Dockerfile` – Defines container build for auth service.
  * **`user-service/`** – NestJS microservice managing user profiles, follows, and preferences.

    * `src/controllers/` – Endpoints for viewing/editing profiles, following users.
    * `src/modules/` – Encapsulates controllers and services into logical units.
    * `src/services/` – Handles database queries and profile business rules.
    * `src/main.ts` – Application entrypoint.
    * `Dockerfile` – Container spec.
  * **`post-service/`** – NestJS microservice powering post creation, feeds, and timeline logic.

    * `src/controllers/` – CRUD routes for posts, likes, comments, and feed retrieval.
    * `src/modules/` – Feature groupings (PostsModule, CommentsModule).
    * `src/services/` – Core post‑management logic, feed algorithms.
    * `src/main.ts` – Starts the service.
    * `Dockerfile` – Builds Docker image.
  * **`ml-service/`** – FastAPI microservice for running ML models and analytics endpoints.

    * `app/routers/` – Route definitions for `/predict`, `/analyze`, etc.
    * `app/models/` – Pydantic schemas for request/response data.
    * `app/services/` – Model loading, inference, data‐prep logic.
    * `app/main.py` – FastAPI application startup.
    * `Dockerfile` – Container build for ML service.

* **`libs/`** – Shared code modules and types used across services.

  * `dto/` – Data‑transfer object definitions (TypeScript interfaces & Pydantic classes) to keep contracts consistent.
  * `auth-utils/` – Shared helpers for token creation, hashing, and validation.
  * `logger/` – Standardized logging setup and formats.

* **`infra/`** – Infrastructure‑as‑Code for provisioning and configuring cloud resources.

  * `terraform/` – Terraform configs (VPC, databases, IAM, managed services).
  * `k8s/` – Kubernetes manifests (Deployments, Services, Ingress rules).

* **`scripts/`** – Utility and automation scripts (build wrappers, deploy shortcuts, codegen).

* **`docker-compose.yml`** – Local development orchestrator that spins up all services (frontend, auth, user, post, ml) and supporting containers (Postgres, Redis) on a shared network.

---

## Contributing

1. Fork the repo  
2. Create a feature branch (`git checkout -b feat/awesome`)  
3. Commit your changes (`git commit -m 'feat: add awesome'`)  
4. Push to your branch (`git push origin feat/awesome`)  
5. Open a Pull Request  

Please follow our [Code of Conduct](CODE_OF_CONDUCT.md) and use the pre-commit hooks for linting and formatting.

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.