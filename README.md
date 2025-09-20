# JobHub - Job Portal Application

A comprehensive job portal application built with React, TypeScript, and Tailwind CSS that connects job seekers with recruiters.

## Features

### 🔍 Job Search & Filtering
- **Search**: Search jobs by title, company, or skills
- **Filter**: Filter by job type, location, and experience level
- **Sort**: Sort jobs by date posted, salary, or title
- **Real-time filtering** with job count indicators

### 👥 User Roles
- **Job Seekers**: Browse and apply for jobs
- **Recruiters**: Post, edit, and manage job listings

### 💼 Job Management
- **CRUD Operations**: Create, read, update, and delete job postings
- **Rich Job Details**: Comprehensive job descriptions, requirements, benefits, and skills
- **Application Tracking**: Track job applications and status

### 🎨 Modern UI/UX
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Clean Interface**: Inspired by modern job portal designs
- **Consistent Design System**: Custom theme with JobHub branding
- **Interactive Components**: Hover effects, transitions, and loading states

## Technical Stack

- **Frontend**: React 18 with TypeScript
- **Styling**: Tailwind CSS with custom design system
- **UI Components**: Shadcn/ui component library
- **State Management**: React Context API
- **Data Fetching**: Custom hooks with React Query
- **Build Tool**: Vite
- **Icons**: Lucide React

## API Integration

The application fetches job data from: `https://jsonfakery.com/jobs`

Mock data is also provided to ensure the application works even if the external API is unavailable.

## Getting Started

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd jobhub
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:8080`

## User Guide

### For Job Seekers
1. **Sign In**: Click "Sign In" and select "Job Seeker"
2. **Browse Jobs**: Use filters and search to find relevant positions
3. **View Details**: Click on any job card to see full details
4. **Apply**: Click "Apply for this Position" to submit your application

### For Recruiters
1. **Sign In**: Click "Sign In" and select "Recruiter"
2. **Manage Jobs**: Use the "Manage Jobs" tab to create and edit listings
3. **Post Jobs**: Click "Post New Job" to create a new job listing
4. **Edit/Delete**: Use the edit and delete buttons on existing jobs

## Architecture

### Component Structure
```
src/
├── components/
│   ├── ui/              # Reusable UI components
│   ├── AuthDialog.tsx   # Authentication modal
│   ├── FilterSidebar.tsx # Job filtering sidebar
│   ├── Header.tsx       # Main navigation header
│   ├── JobCard.tsx      # Individual job listing card
│   ├── JobDetail.tsx    # Detailed job view
│   └── JobManagement.tsx # Recruiter job management
├── contexts/
│   └── AuthContext.tsx  # Authentication state management
├── hooks/
│   ├── useJobs.ts       # Job data fetching and management
│   └── use-toast.ts     # Toast notifications
├── lib/
│   └── jobUtils.ts      # Utility functions for job data
├── types/
│   └── job.ts           # TypeScript type definitions
└── pages/
    └── Index.tsx        # Main application page
```

### Design System
- **Colors**: Custom JobHub blue theme with semantic color tokens
- **Typography**: System fonts with consistent sizing and weights
- **Spacing**: Consistent spacing scale using Tailwind utilities
- **Components**: Custom variants for buttons and other UI elements

## Features Implementation

✅ **Add, update, delete, and sort job postings** - Full CRUD operations for recruiters
✅ **View job descriptions in detail** - Comprehensive job detail view
✅ **User roles (Recruiter / Job Seeker)** - Role-based authentication and features
✅ **Job application system** - Job seekers can apply for positions
✅ **Search, Filter, and Sort** - Multiple ways to find relevant jobs
✅ **Real-time job counts** - Filter indicators show available job counts
✅ **Responsive design** - Works on all device sizes
✅ **Modern UI/UX** - Clean, professional interface
✅ **API integration** - Fetches data from provided endpoint

## Bonus Features

- **Application tracking** - Users can see which jobs they've applied to
- **Toast notifications** - User feedback for all actions
- **Loading states** - Proper loading indicators
- **Error handling** - Graceful error handling and retry mechanisms
- **Accessibility** - Semantic HTML and keyboard navigation
- **SEO optimized** - Proper meta tags and structured content

## Future Enhancements

- User profiles and resume upload
- Advanced search with salary range filtering
- Email notifications for new jobs
- Company profiles and ratings
- Job alerts and saved searches
- Application status tracking
- Interview scheduling

## License

This project is built for demonstration purposes as part of a job portal application assessment.