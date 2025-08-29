# 🌱 CropIT - The URL Shortener That Doesn't Cut Corners

## 🚀 Overview

**CropIT** is a modern, feature-rich URL shortening service built with Next.js, offering an intuitive interface for shortening, managing, and tracking your links. This project was developed as a mini-project for our college classes by:

- [Abhishek Singh](https://github.com/AbhishekS04) - The code wrangler who believes indentation is a love language
- [Snehasish Mondal](https://github.com/Snehasish321) - The UI wizard who once fixed a bug by turning his laptop off and on again

## ✨ Features

- **🔗 URL Shortening**: Transform those embarrassingly long URLs into sleek, shareable links
- **🔍 Custom Short Codes**: Create memorable, branded links with custom codes
- **📊 Analytics Dashboard**: Track clicks and view statistics for your shortened URLs
- **👤 User Authentication**: Register and login to keep all your shortened URLs in one place
- **🔒 Admin Dashboard**: Moderate URLs, manage users, and keep things running smoothly
- **🚦 URL Flagging System**: Automatic detection of potentially suspicious URLs
- **📱 Responsive Design**: Works perfectly on devices of all sizes (even that ancient phone your grandma uses)
- **🌓 Dark/Light Mode**: Because eye strain is so last season
- **📱 QR Code Generation**: Generate QR codes for your shortened URLs

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 19, Tailwind CSS, shadcn/ui
- **Backend**: Next.js API Routes
- **Database**: PostgreSQL with Drizzle ORM
- **Authentication**: NextAuth.js
- **Validation**: Zod
- **Analytics**: Custom tracking system with Recharts for visualization
- **Hosting**: Ready to deploy on Vercel

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/AbhishekS04/CropIT.git
   cd CropIT
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   # or
   bun install
   ```

3. **Set up environment variables**
   ```
   # Create a .env.local file with these variables
   DATABASE_URL=your_postgres_connection_string
   NEXTAUTH_SECRET=your_secret_key
   NEXTAUTH_URL=http://localhost:3000
   GOOGLE_GENERATIVE_AI_API_KEY=your_gemini_api_key
   ```

4. **Initialize the database**
   ```bash
   npx drizzle-kit push:pg
   ```

5. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   # or
   bun dev
   ```

6. **Open [http://localhost:3000](http://localhost:3000)** and start cropping those URLs! 🌱

## 📁 Project Structure

```
CropIT/
├── src/
│   ├── app/                 # Next.js App Router
│   │   ├── (admin)/         # Admin dashboard routes
│   │   ├── (auth)/          # Authentication routes
│   │   ├── (user)/          # User dashboard routes
│   │   └── page.tsx         # Home page
│   ├── components/          # Reusable components
│   │   ├── ui/              # shadcn/ui components
│   │   ├── auth/            # Authentication components
│   │   ├── admin/           # Admin-specific components
│   │   └── urls/            # URL-related components
│   ├── lib/                 # Utility functions and types
│   └── server/              # Server actions and auth
├── drizzle/                 # Database migrations
└── public/                  # Static assets
```

## 🎯 Key Features Explained

### URL Shortening
Simply paste any URL into our form, and CropIT will generate a short, shareable link. You can also customize the ending with your own code for branding!

### Smart URL Detection
Our AI-powered system can detect potentially suspicious URLs and flag them for review, keeping the platform safe for everyone.

### User Dashboard
Registered users get access to a personal dashboard where they can:
- View all their shortened URLs
- Track click statistics
- Edit or delete links
- Generate QR codes

### Admin Panel
Administrators can:
- Manage all URLs on the platform
- Review flagged content
- Manage user accounts
- Access detailed analytics

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change. We're particularly interested in:

- New feature implementations
- Bug fixes
- UI/UX improvements
- Performance optimizations

Remember, the best code is written after midnight with at least three energy drinks. (Just kidding, please prioritize your health and sleep.)

## 🐛 Known Issues

- Sometimes the app works so fast that users don't believe their URL was actually shortened
- Our analytics are so detailed they might make Google Analytics jealous
- The dark mode is so dark that users have reported losing their cursor in it

## 🎯 Future Plans

- Mobile app development
- Browser extensions
- Advanced analytics
- Custom QR code styling
- Enterprise features
- World domination (just kidding... or are we?)

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- Our professors who pretended to understand our technical explanations
- Stack Overflow for being our second home
- Coffee shops with reliable WiFi
- The inventors of caffeine

---

<div align="center">
  <p>Made with ❤️ and <strong>way too much</strong> caffeine</p>
  <p>© 2025 CropIT Team | <a href="https://github.com/AbhishekS04">Abhishek</a> & <a href="https://github.com/Snehasish321">Snehasish</a></p>
</div>
