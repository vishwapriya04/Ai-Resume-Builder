# AI-Powered Resume Builder

A modern, full-featured resume builder with AI-powered suggestions and multiple input methods.

## Features

### Input Methods
- **Form-based input**: Build your resume section by section with intuitive form fields
- **File upload**: Import existing resumes (TXT, PDF, DOCX)
- **Text paste**: Copy/paste resume content directly
- **Auto-save**: Your resume is automatically saved to browser storage

### Resume Sections
- **Personal Information**: Name, email, phone, location, and professional summary
- **Experience**: Add multiple positions with company, title, dates, and descriptions
- **Education**: Track degrees, schools, fields of study, and graduation years
- **Skills**: Manage and organize your technical and professional skills

### AI Features
- **Smart Suggestions**: Get AI-powered recommendations for:
  - Improving bullet points with metrics and impact
  - Enhancing professional summaries
  - Suggesting relevant skills
  - Optimizing achievement statements
- **Real-time API Integration**: Suggestions powered by API endpoint at `/api/suggestions`

### Preview & Export
- **Live Preview**: See your resume in professional formatting as you edit
- **Print to PDF**: Export your resume as a PDF with professional styling
- **Clean Design**: Modern, ATS-friendly resume template

### Data Management
- **Local Storage**: Resume data persists across browser sessions
- **Clear All**: Reset to default resume and clear all data
- **Responsive Design**: Works seamlessly on desktop and tablet devices

## Technical Stack
- **Frontend**: Next.js 16 with React 19
- **Styling**: Tailwind CSS with custom design tokens
- **Components**: shadcn/ui component library
- **State Management**: React hooks with localStorage persistence
- **File Handling**: Client-side resume parsing utilities
- **Icons**: Lucide React

## File Structure
```
components/
  ├── resume-builder.tsx      # Main form component
  ├── resume-preview.tsx      # Professional resume display
  └── file-upload.tsx         # File import interface

lib/
  ├── storage.ts              # LocalStorage utilities
  ├── file-parser.ts          # Resume parsing logic
  ├── ai-client.ts            # AI suggestion API client
  └── utils.ts                # Common utilities

hooks/
  └── use-pdf-export.ts       # PDF export functionality

app/
  ├── page.tsx                # Main application page
  └── api/
      └── suggestions/
          └── route.ts        # AI suggestions API endpoint

types/
  └── resume.ts               # TypeScript interfaces
```

## Getting Started

1. Run the development server:
   ```bash
   npm run dev
   ```

2. Open [http://localhost:3000](http://localhost:3000) in your browser

3. Start building your resume using the form, preview it, and export as PDF

## Future Enhancements

- Integration with real AI APIs (OpenAI, Anthropic, etc.)
- PDF parsing library for better document import
- Multiple resume templates
- Collaboration features
- Cloud storage sync
- Resume analytics and ATS optimization
