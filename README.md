# JobVibes
Welcome to **JobVibes** – a place to share and read honest, anonymous workplace experiences.
Ever wondered, **“Should I work here?”** Now you can find out.

---

## What is JobVibes?
JobVibes is a simple web app where people can:
- Leave **anonymous reviews** about their workplace.
- **Search for companies** to see what others are saying.
- Help job seekers get a real sense of the **vibe** at a company before they apply.

Whether it’s the pay, the culture, or that one manager everyone loves (or doesn’t), JobVibes makes it easy to share your thoughts without revealing your name.

---

## Tech Stack
We’re keeping things modern and lightweight:

**Frontend**
- **React** – Makes the app fast and dynamic.
- **Tailwind CSS** – Keeps things clean and responsive.

**Backend**
- **Node.js + Express** – Handles reviews and API requests.
- **MongoDB (Atlas)** – Stores all the company reviews securely in the cloud.

**Hosting**
- **Vercel / Netlify** – Free hosting for the frontend.
- **Render / Railway** – Free hosting for the backend.

---

## How It’s Organized
```
jobvibes/
  frontend/
    src/
      components/
      pages/
      App.js
  backend/
    server.js
    routes/
      reviews.js
    models/
      Review.js
```

---

## MVP Features
Here’s what the first version of JobVibes will do:

1. **Landing Page**
   - Simple welcome page with a **search bar**: “Search for a company…”
   - A button to see what people are saying.

2. **Company Review Pages**
   - List of **anonymous reviews** with star ratings, like:
     ```
     ★★★★☆  “Great pay but long hours.”
     ★★★☆☆  “Management could improve.”
     ```
   - A button to **leave your own review**.

3. **Submit Review Page**
   - A quick form:
     - Company Name
     - 1–5 Star Rating
     - Your Review
   - Optionally add a nickname (or stay 100% anonymous).

4. **Basic API**
   - `GET /reviews` → Get all reviews
   - `POST /reviews` → Add a new review

---

## Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/yourusername/jobvibes.git
cd jobvibes
```

### 2. Setup Backend
```bash
cd backend
npm install
npm start
```
- Don’t forget to add your MongoDB connection string in a `.env` file!

### 3. Setup Frontend
```bash
cd frontend
npm install
npm run dev
```

Open `http://localhost:5173` (or whatever Vite gives you) to see JobVibes in action.

---

## What’s Next?
- Add upvotes and comments to reviews.
- Search and filter companies.
- Optional user accounts to track your reviews.
- Launch the live site so people can start sharing vibes.
