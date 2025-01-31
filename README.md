---

# Support Desk System

This repository hosts the **Support Desk System**, a project designed to simplify issue tracking, solution sharing, and report generation. The system consists of two main components:

- **Backend**: Built with [NestJS](https://nestjs.com/), integrated with MongoDB for database management, and containerized with Docker.
- **Frontend**: Developed using [Next.js](https://nextjs.org/) for a seamless user interface and experience.

## Features

- **User-friendly Forum**: CRUD operations for managing problems, solutions, and logs.
- **Reporting**: Generate detailed reports on issues and resolutions.
- **Scalable Design**: Modular architecture for future enhancements.
- **Cross-Platform**: Accessible via desktop and mobile browsers.

---

## System Architecture

### 1. **Frontend**

- Built with **Next.js**
- Provides a responsive UI
- Communicates with the backend via REST APIs

### 2. **Backend**

- Built with **NestJS**
- Handles business logic and API requests
- Uses **MongoDB** for data storage
- Containerized using **Docker** for easy deployment

---

## Installation & Setup

### Prerequisites

- Node.js (>= v16.x)
- Docker (if running the backend as a container)

### Clone the Repository

```bash
git clone https://github.com/<your-org-name>/support-desk-system.git
cd support-desk-system
```

### Backend Setup

1.Navigate to the `backend` directory:

```bash
cd backend
```

2.Install dependencies:

```bash
npm install
```

3.Configure environment variables:

- Create a `.env` file in the `backend` directory.
- Add the necessary variables (example provided in `.env.example`).

  4.Start the server:

- Locally:

```bash
npm run start:dev
```

- Using Docker:

```bash
docker-compose up
```

### Frontend Setup

1.Navigate to the `frontend` directory:

```bash
cd ../frontend
```

2.Install dependencies:

```bash
npm install
```

3.Configure environment variables:

- Create a `.env.local` file in the `frontend` directory.
- Add the necessary variables (example provided in `.env.local.example`).
  4.Start the development server:

```bash
npm run dev
```

---

## Usage

1. Open the browser and navigate to `http://localhost:3000` to access the frontend.
2. Backend runs by default on `http://localhost:5000` (or Docker's exposed port).
3. Explore the following key features:
   - **Forum**: Add, edit, or delete problems, solutions, and logs.
   - **Reports**: Generate comprehensive issue reports.

---

## Deployment

For deployment, follow these steps:

1. Build the frontend:

```bash
npm run build
```

2. Use Docker Compose to deploy the entire system:

```bash
docker-compose -f docker-compose.prod.yml up --build
```

---

## Contributing

We welcome contributions! Please:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`.
3. Commit your changes: `git commit -m "Add your feature"`.
4. Push the branch: `git push origin feature/your-feature`.
5. Open a Pull Request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For inquiries, please contact **<your-org-email@example.com>**.

---
