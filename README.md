<div align="center">
  <img src="./Roomiebu%20just%20the%20logo.png" alt="RoomiesBU Logo" width="120" />
  <h1>RoomiesBU</h1>
  <p>Find your perfect roommate at Stony Brook University before the semester even starts! 🍕📚</p>
  
  [![Live Demo](https://img.shields.io/badge/Live_Demo-roomiebu.vercel.app-000000?style=for-the-badge&logo=vercel)](https://roomiebu.vercel.app/)
</div>

## 📌 What is RoomiesBU?

Let's be real—getting randomly assigned a roommate can be a massive gamble. You might be a hardcore CS major who wants absolute silence, and your roommate might be throwing a party at 3 AM. 

**RoomiesBU** fixes that. I built this platform so you can vibe-check your potential roommates *before* you move in. 

- Want a roommate who is vegetarian, eggitarian, or non vegetarian? Done. 
- Looking for someone who doesn't smoke? Easy. 
- Need a fellow B.Tech student to suffer through assignments with? You'll find them here.

Whether you're looking for a lively party scene or a silent sanctuary to sleep, RoomiesBU helps you filter and find your perfect match.

## 📈 Traction & Impact (Real World Usage)
Since launch, the platform has seen incredible engagement from the student body:
- **570+ Active Users** onboarded.
- **155+ Room/Roommate Listings** posted.
- **500+ Interests (Connect Requests)** sent between users.
- **100+ Successful Matches** made!

## 🚀 Features

- **Vibe-Check Filters:** Filter profiles by smoking habits, diet (Veg/Non-veg), noise preferences (Party Animal vs. Silent Room), and course (like B.Tech).
- **Secure University Authentication:** Login safely using your university Google or Microsoft Entra ID. No randoms allowed.
- **Real-Time Notifications:** Integrated with Resend so you get an email the second you get a match.
- **Lightning Fast UI:** Built with Next.js, because nobody has time for slow websites.

## 🛠️ Tech Stack

- **Framework:** [Next.js](https://nextjs.org/)
- **Database:** PostgreSQL via [Prisma ORM](https://www.prisma.io/)
- **Authentication:** [NextAuth.js](https://next-auth.js.org/) (Google & Microsoft)
- **Emails:** [Resend](https://resend.com/)
- **Deployment:** [Vercel](https://vercel.com)

## 💻 Running Locally (For Devs & Interviewers)

Want to run this on your own machine? Here is the step-by-step:

### 1. Clone the repository
```bash
git clone https://github.com/your-username/roomiesbu.git
cd roomiesbu
```

### 2. Install dependencies
```bash
npm install
```

### 3. Set up Environment Variables (`.env`)
*(Note: To see exactly which variables this project needs, look at the `.env.example` file included in this repository!)*

1. Copy the `.env.example` file and rename it to `.env`:
   ```bash
   cp .env.example .env
   ```
2. Open the `.env` file and fill in your database URLs and API keys. 
3. **If you are an interviewer or recruiter:** Please reach out to me directly and I will gladly provide you with a secure set of staging credentials so you can test it easily!

### 4. Setup the Database
Generate the Prisma client and push the schema to your local database:
```bash
npx prisma generate
npx prisma db push
```

### 5. Start the Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) with your browser to see the app in action.
