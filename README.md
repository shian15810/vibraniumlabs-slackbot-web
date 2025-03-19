# Take Home Exercise: Slack Bot 🤖

## Objective:

Develop an interactive dashboard and Slack bot that integrates with OpenAI’s GPT API to provide intelligent, context-aware responses to user queries. The dashboard should offer insights into query trends, user engagement, and common topics, serving as a monitoring and analytics tool for interactions with the bot.

You are expected to spend up to 48 hours on the exercise, and you are *not* expected to complete all of the requirements below. Given the scope of features, you will need to prioritize, design, and develop key functionalities, making thoughtful trade-offs to deliver a well-structured, high-impact solution.

As an AI-first company, we encourage the use of tools like Cursor, ChatGPT, and other AI-assisted development resources to enhance efficiency and productivity.

## Requirements:

### **Backend:**

- **Slack Integration:**
    - Set up a bot that listens to messages in a Slack channel.
    - The bot should first attempt to answer questions based on past Slack threads before falling back to general knowledge from OpenAI’s GPT model.
- **OpenAI API Integration:**
    - Process user queries and generate appropriate responses.
    - Support retrieval-augmented generation (RAG) by leveraging relevant past conversations and tools like [pinecone.io](http://pinecone.io).
- **Uploaded Files as Context:**
    - Allow users to upload files that the model can reference when answering questions.
    - Extract text from uploaded documents (e.g., PDFs, CSVs, or text files) and include this information in query responses.
- **Data Logging & Storage:**
    - Store query data, responses, timestamps, and metadata to generate insights.
    - Store Slack messages for historical context and better query responses.

### **Frontend (Dashboard UI):**

- **React-Based Interface:**
    - Use React (TypeScript preferred) with Next.js, Vite, etc. for frontend development.
    - Build a responsive and interactive UI for monitoring query insights.
- **Metrics Dashboard:**
    
    Display key statistics on the queries made via the Slack bot, including:
    
    - **Hot Keywords:** Show the most frequently used keywords across all queries.
    - **Trend Over Time:** Chart how query volume and keyword popularity change over time.
    - **Top Users:** Rank users by the number of queries made.
    - **User Query Trends:** Show individual user engagement trends over time.
    - **Response Effectiveness:** Track how often the bot resolves queries without requiring human intervention.
- **Chat Interface:**
    - Enable users to interact with the bot directly via the dashboard.
    - Provide a chat history with timestamps, showing past queries and responses.
    - Allow users to input queries and get responses without using Slack.
- **File Upload & Context Usage:**
    - Implement a file upload feature to let users provide additional context for queries.
    - Display uploaded files and allow users to see how they influence responses.
- **Slack Message Summarization:**
    - Display summarized Slack conversations and extracted insights.
    - Provide a searchable history of Slack conversations relevant to specific keywords.

### **Nice-to-Have’s:**

- **Testing:**
    - Write unit and/or integration tests for both frontend and backend.
- **Deployment:**
    - Deploy frontend using Vercel and backend using Heroku/AWS/GCP.
- **Authentication:**
    - Implement basic authentication via Slack OAuth or simple login.
- **Additional Features:**
    - It’s really up to your imagination. Sky is the limit!

We are very excited to see what you can accomplish with this exercise. Most importantly, have fun with it!

👉 When completed, please reach out to Charles ([charles@vibraniumlabs.ai](mailto:charles@vibraniumlabs.ai)), cc Jay ([jay@vibraniumlabs.ai](mailto:jay@vibraniumlabs.ai)) and Reese ([reese@t1.co](mailto:reese@t1.co)) and share the link to your repository for the exercise. Charles will then set up a 30 minute debrief/demo. Good luck!

---

This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
