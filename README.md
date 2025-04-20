# Viral_Reels_Script_Generator

# Viral Reels Script Generator (MVP)

Welcome to the **Viral Reels Script Generator** project! This is a simple MVP that generates scripts for viral reels, including captions, hashtags, voiceovers, and trending sound suggestions. The app uses **DeepSeek API** for text generation, **PlayHT** for text-to-speech, **MongoDB Atlas** for storage, and **Clerk.dev** for authentication.

## 🧰 **Tech Stack**

- **Frontend**: Next.js (React), Tailwind CSS
- **Backend**: Node.js, Express.js, Vercel Serverless Functions
- **Database**: MongoDB Atlas
- **Authentication**: Clerk.dev
- **AI Services**: DeepSeek API (Text Generation), PlayHT (Text-to-Speech)
- **Hosting & Deployment**: Vercel
- **Version Control**: Git, GitHub

## 🚀 **Getting Started**

Follow these steps to set up the project locally.

### 1. **Check if Node.js & npm are installed**

First, check if **Node.js** and **npm** are installed by running:

```bash
node -v
npm -v
If not installed, run the following command to install them:

bash
Copy
Edit
winget install OpenJS.NodeJS.LTS
2. Check if Git is installed
Ensure Git is installed by running:

bash
Copy
Edit
git --version
If not installed, run:

bash
Copy
Edit
winget install Git.Git
3. Clone the Repository
Clone this repository to your local machine:

bash
Copy
Edit
git clone https://github.com/your-username/viral-reels-mvp.git
cd viral-reels-mvp
4. Install Dependencies
Install the required project dependencies:

bash
Copy
Edit
npm install
If you prefer using Yarn, install it globally and then use it to install dependencies:

bash
Copy
Edit
npm install --global yarn
yarn install
5. Set Up MongoDB Connection (Optional for Local Dev)
If using MongoDB Atlas, follow these steps:

Create a free cluster on MongoDB Atlas.

Whitelist IP: 0.0.0.0/0 (for development purposes).

Create a DB user and note the password.

Copy your connection string (e.g., mongodb+srv://user:pass@cluster.mongodb.net/dbname).

Add the connection string to the .env.local file:

bash
Copy
Edit
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/dbname
6. Set Up Clerk.dev Authentication
Sign up at Clerk.dev.

Create an application and copy your Frontend API and Publishable Key.

Add the keys to your .env.local file:

bash
Copy
Edit
CLERK_FRONTEND_API=your_clerk_frontend_api
CLERK_PUBLISHABLE_KEY=your_publishable_key
7. Set Up DeepSeek API
Sign up at DeepSeek.

Copy your API Key.

Add it to .env.local:

bash
Copy
Edit
DEEPSEEK_API_KEY=your_deepseek_api_key
8. Set Up PlayHT (TTS)
Sign up at PlayHT.

Go to the dashboard, and retrieve your User ID and Secret Key from the API section.

Add them to .env.local:

bash
Copy
Edit
PLAYHT_USER_ID=your_id
PLAYHT_API_KEY=your_key
9. Run the Development Server
Once everything is set up, you can start the development server:

bash
Copy
Edit
npm run dev
Visit http://localhost:3000 to view the app.

🔐 Environment Variables
Make sure the following environment variables are added to your .env.local file:

bash
Copy
Edit
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/dbname
CLERK_FRONTEND_API=your_clerk_frontend_api
CLERK_PUBLISHABLE_KEY=your_publishable_key
DEEPSEEK_API_KEY=your_deepseek_api_key
PLAYHT_USER_ID=your_id
PLAYHT_API_KEY=your_key
⚙️ Development Notes
The project is designed for rapid prototyping and low-cost testing.

We are using DeepSeek for text generation and PlayHT for voiceovers in this MVP.

The backend runs as a serverless function on Vercel, so no infrastructure management is required.

🛠️ Optional Enhancements
Add ESLint and Prettier to ensure code quality and consistency.

Set up a GitHub repo and push your changes for version control.

Install VS Code (optional but recommended for devs):

bash
Copy
Edit
winget install Microsoft.VisualStudioCode
🤖 AI Features Overview
Text Generation: Uses DeepSeek API to generate scripts in the format of Hook → Body → CTA based on user input.

Text-to-Speech (TTS): PlayHT API is used to convert the generated scripts into audio for voiceovers.

Trending Sound Suggestions: Curated list updated weekly for suggested sounds.

📣 Contributing
We welcome contributions! Please fork the repository, make your changes, and submit a pull request.

📅 Roadmap
MVP Features:

Script Generator (DeepSeek)

B-Roll Prompt Suggestions

Caption & Hashtag Generator

Voiceover Generation (PlayHT)

CSV Export for Manual Scheduling

User Authentication (Clerk.dev)

30-Day Niche Content Packs (hardcoded)

Future Features (after monetization):

GPT-4 Integration

Auto-scheduling for Reels

Real-time Trending APIs

Performance Analytics for Hooks

🚀 Ready to Start?
Get the project up and running quickly by following the steps above. If you need help, feel free to open an issue or contact the project maintainers.

🎉 Let’s get this MVP off the ground!
yaml
Copy
Edit

---

This README provides a comprehensive guide for developers to get up and running with your project. It covers everything from tech stack details to the setup process and environment variable configuration. Let me know if you need further tweaks or additions!







