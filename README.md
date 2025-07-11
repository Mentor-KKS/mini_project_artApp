# 🎨 Art Institute Explorer

A React application for exploring and saving artworks from the Art Institute of Chicago collection.

## 📋 Project Overview

This project allows users to:

- Search through the Art Institute of Chicago's extensive art collection
- Save favorite artworks to a personal gallery
- Add personal notes to saved artworks
- View artwork details including artist, date, medium, and dimensions

## 🚀 Tech Stack

- **React** with **TypeScript** for type safety
- **Vite** for fast development and building
- **Zod** for runtime data validation
- **Art Institute of Chicago API** for artwork data
- **localStorage** for persistent data storage

## 📦 Installation

```bash
# Clone the repository
git clone git@github.com:Mentor-KKS/mini_project_artApp.git
cd mini_project_artApp

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

## 🛠️ Available Scripts

```bash
# Development
pnpm dev          # Start development server
pnpm build        # Build for production
pnpm preview      # Preview production build
pnpm lint         # Run ESLint
```

## 🏗️ Project Structure

```
src/
├── components/               # React components
│   ├── ArtworkCard.tsx       # Individual artwork display
│   ├── Gallery.tsx           # Saved artworks collection
│   ├── SearchInterface.tsx   # Search functionality
│   └── Layout.tsx            # App layout wrapper
├── lib/                      # Utility functions
│   ├── api.ts                # API integration
│   ├── schemas.ts            # Zod validation schemas
│   └── storage.ts            # localStorage utilities
├── types/                    # TypeScript type definitions
│   └── index.ts
├── hooks/                    # Custom React hooks
│   └── useLocalStorage.ts
├── App.tsx                   # Main app component
└── main.tsx                  # App entry point
```

## 🎯 Functional Requirements

### ✅ Completed Features

- [x] **FR001**: React + Vite (TypeScript) Setup
- [x] **FR002**: Zod dependency installation
- [ ] **FR003**: Artwork Zod Schema with validation
- [ ] **FR004**: API fetch with data validation
- [ ] **FR005**: Search interface for artwork queries
- [ ] **FR006**: ArtworkCard component for displaying art
- [ ] **FR007**: Gallery component for saved artworks
- [ ] **FR008**: Add artwork to gallery (localStorage)
- [ ] **FR009**: Display saved artworks in gallery
- [ ] **FR010**: Add/edit notes for saved artworks
- [ ] **FR011**: Remove artworks from gallery
- [ ] **FR012**: Type-safe state management

## 🔌 API Integration

This project uses the [Art Institute of Chicago API](https://api.artic.edu/docs/):

### Key Endpoints:

- **Search**: `https://api.artic.edu/api/v1/artworks/search`
- **Images**: `https://www.artic.edu/iiif/2/{image_id}/full/843,/0/default.jpg`

### Data Validation:

All API responses are validated using Zod schemas to ensure type safety and handle missing data gracefully.

## 💾 Data Storage

- **Gallery**: Saved artworks stored in `localStorage`
- **Notes**: Personal notes for each artwork stored locally
- **Persistence**: Data persists between browser sessions

## 🎨 Features

### Search Interface

- Search the Art Institute's collection by keywords
- View search results with artwork previews
- Filter and browse through results

### Personal Gallery

- Save favorite artworks to your personal collection
- Add personal notes and thoughts about each piece
- Remove artworks from your gallery
- Persistent storage across sessions

### Artwork Details

- High-quality images from the Art Institute's IIIF service
- Artist information and artwork titles
- Creation dates and medium information
- Artwork dimensions and additional metadata

## 🔧 Development Notes

### Type Safety

- All components use TypeScript for compile-time type checking
- Zod schemas provide runtime validation
- Type inference from Zod schemas ensures consistency

### Error Handling

- API failures are handled gracefully
- Invalid data is filtered out or assigned default values
- User feedback for loading states and errors

### Performance

- Lazy loading for artwork images
- Efficient re-renders with proper React patterns
- Optimized API calls with debouncing

## 📚 Learning Objectives

This project demonstrates:

- **Third-party API integration** with proper error handling
- **Data validation** using Zod schemas
- **TypeScript** for type-safe React development
- **State management** with React hooks
- **localStorage** for client-side persistence
- **Component composition** and reusability

## 🌟 Future Enhancements

- Advanced search filters (by artist, date, medium)
- Export gallery as PDF or image collection
- Social sharing of favorite artworks
- Advanced note-taking with rich text
- Artwork comparison features
- Integration with other museum APIs

## 📄 License

This project is for educational purposes as part of a coding bootcamp curriculum.

## 🙏 Acknowledgments

- [Art Institute of Chicago](https://www.artic.edu/) for providing the open API
- [Vite](https://vitejs.dev/) for the excellent development experience
- [Zod](https://zod.dev/) for runtime type validation

---
