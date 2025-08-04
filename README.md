# ALX Movie App

A modern movie discovery application built with Next.js 14, TypeScript, and Tailwind CSS. Discover, explore, and enjoy movies from around the world using The Movie Database (TMDB) API.

## 🎬 Features

- **Movie Discovery**: Browse popular and trending movies
- **Advanced Search**: Find movies by title with real-time search
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Modern UI**: Clean and intuitive interface with Tailwind CSS
- **Movie Cards**: Detailed movie information with posters, ratings, and descriptions
- **Pagination**: Navigate through extensive movie collections
- **Font Awesome Icons**: Beautiful and consistent iconography

## 🛠️ Tech Stack

- **Framework**: Next.js 14 (Pages Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Icons**: Font Awesome
- **API**: The Movie Database (TMDB)
- **Package Manager**: npm

## 📁 Project Structure

```bash
alx-movie-app/
├── components/
│   ├── commons/
│   │   ├── Button.tsx
│   │   ├── Loading.tsx
│   │   └── MovieCard.tsx
│   └── layouts/
│       ├── Footer.tsx
│       ├── Header.tsx
│       └── Layout.tsx
├── interfaces/
│   └── index.ts
├── pages/
│   ├── api/
│   │   └── fetch-movies.ts
│   ├── movies/
│   │   └── index.tsx
│   ├── _app.tsx
│   └── index.tsx
├── public/
├── styles/
│   └── globals.css
├── .env.local
├── .eslintrc.json
├── .gitignore
├── next.config.ts
├── package.json
└── tsconfig.json
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- TMDB API key

### Installation

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd alx-project-0x14/alx-movie-app
   ```

1. **Install dependencies:**

   ```bash
   npm install
   ```

1. **Set up environment variables:**
   Create a `.env.local` file in the root directory and add your TMDB API key:

   ```env
   TMDB_API_KEY=your_tmdb_api_key_here
   ```

   Get your API key from [The Movie Database (TMDB)](https://www.themoviedb.org/settings/api)

4. **Run the development server:**

   ```bash
   npm run dev
   ```

5. **Open your browser:**
   Navigate to [http://localhost:3000](http://localhost:3000) to see the application.

## 🔧 Available Scripts

- `npm run dev` - Start the development server
- `npm run build` - Build the application for production
- `npm run start` - Start the production server
- `npm run lint` - Run ESLint for code linting

## 🎯 Usage

### Home Page

- View featured movies from TMDB
- Navigate to the movies page for full exploration
- Responsive hero section with call-to-action buttons

### Movies Page

- Browse popular movies
- Search for specific movies using the search bar
- Navigate through pages of results
- Click on movie cards for detailed information

### API Routes

- `/api/fetch-movies` - Fetch movies from TMDB with optional search and pagination

## 🌟 Components

### Common Components

- **Button**: Reusable button with multiple variants and sizes
- **Loading**: Animated loading spinner with Font Awesome
- **MovieCard**: Movie display component with poster, title, rating, and overview

### Layout Components

- **Header**: Navigation header with app branding and menu
- **Footer**: Application footer with links and social media
- **Layout**: Main layout wrapper component

## 🔑 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `TMDB_API_KEY` | The Movie Database API key | Yes |

## 📱 Responsive Design

The application is fully responsive and optimized for:

- **Desktop**: Full-featured experience with grid layouts
- **Tablet**: Adapted layouts for medium screens
- **Mobile**: Touch-friendly interface with stacked layouts

## 🎨 Styling

- **Tailwind CSS**: Utility-first CSS framework
- **Custom Utilities**: Line clamping and smooth transitions
- **Dark Mode**: System preference-based dark mode support
- **Color Scheme**: Modern blue and gray color palette

## 🚀 Deployment

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out the [Next.js deployment documentation](https://nextjs.org/docs/pages/building-your-application/deploying) for more details.

## 📝 License

This project is part of the ALX Software Engineering Program.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📞 Support

For support and questions, please refer to the ALX Software Engineering Program resources or create an issue in the repository.

## TMDB API Documentation

## API Overview

The Movie Database (TMDB) API is a comprehensive REST API that provides access to an extensive collection of movie and TV show information. TMDB offers detailed metadata including cast information, plot summaries, release dates, ratings, images, and much more. The API serves as the backbone for countless movie and entertainment applications worldwide.

Key features of the TMDB API include:

- **Comprehensive Movie Database**: Access to millions of movies with detailed metadata
- **TV Show Information**: Complete TV series data including episodes and seasons  
- **People & Cast Details**: Actor, director, and crew information with biographies
- **Rich Media Content**: High-quality posters, backdrops, and promotional images
- **Search Capabilities**: Powerful search functionality across all content types
- **Real-time Updates**: Regular updates with the latest releases and information
- **Multiple Languages**: Support for multiple languages and localization
- **User Ratings & Reviews**: Community-driven ratings and user-generated reviews

## API Version

### Current Version: 3

TMDB API version 3 is the current stable version that provides comprehensive access to all movie and TV show data. This version uses RESTful endpoints and returns JSON responses. Version 4 is also available but version 3 remains the recommended choice for most applications due to its stability and extensive documentation.

## Available Endpoints

### Movies

- **GET `/movie/popular`** - Get a list of movies ordered by popularity
- **GET `/movie/top_rated`** - Get top-rated movies  
- **GET `/movie/now_playing`** - Get movies currently in theaters
- **GET `/movie/upcoming`** - Get upcoming movie releases
- **GET `/movie/{movie_id}`** - Get detailed information about a specific movie
- **GET `/movie/{movie_id}/credits`** - Get cast and crew for a movie
- **GET `/movie/{movie_id}/images`** - Get movie posters and backdrops
- **GET `/movie/{movie_id}/videos`** - Get trailers and video content
- **GET `/movie/{movie_id}/reviews`** - Get user reviews for a movie
- **GET `/movie/{movie_id}/similar`** - Get similar movies

### Search

- **GET `/search/movie`** - Search for movies by title
- **GET `/search/tv`** - Search for TV shows
- **GET `/search/person`** - Search for actors, directors, and other people
- **GET `/search/multi`** - Search across all content types

### TV Shows

- **GET `/tv/popular`** - Get popular TV shows
- **GET `/tv/top_rated`** - Get top-rated TV shows
- **GET `/tv/{tv_id}`** - Get detailed TV show information
- **GET `/tv/{tv_id}/season/{season_number}`** - Get specific season details

### People

- **GET `/person/popular`** - Get popular people in entertainment
- **GET `/person/{person_id}`** - Get detailed person information
- **GET `/person/{person_id}/movie_credits`** - Get person's movie appearances

### Configuration

- **GET `/configuration`** - Get API configuration including image base URLs
- **GET `/genre/movie/list`** - Get list of movie genres
- **GET `/genre/tv/list`** - Get list of TV genres

## Request and Response Format

### Request Structure

All API requests follow a consistent RESTful format:

```bash
GET https://api.themoviedb.org/3/{endpoint}?api_key={your_api_key}
```

**Example Request:**

```bash
curl --request GET \
  --url 'https://api.themoviedb.org/3/movie/popular?api_key=YOUR_API_KEY&language=en-US&page=1' \
  --header 'accept: application/json'
```

### Response Structure

API responses are returned in JSON format with a consistent structure:

**Movies List Response:**

```json
{
  "page": 1,
  "results": [
    {
      "adult": false,
      "backdrop_path": "/path/to/backdrop.jpg",
      "genre_ids": [28, 12, 878],
      "id": 550,
      "original_language": "en",
      "original_title": "Fight Club",
      "overview": "A depressed man joins a fight club...",
      "popularity": 61.115,
      "poster_path": "/path/to/poster.jpg",
      "release_date": "1999-10-15",
      "title": "Fight Club",
      "video": false,
      "vote_average": 8.433,
      "vote_count": 26279
    }
  ],
  "total_pages": 42635,
  "total_results": 852688
}
```

**Movie Details Response:**

```json
{
  "id": 550,
  "title": "Fight Club",
  "overview": "A depressed man joins a fight club...",
  "release_date": "1999-10-15",
  "runtime": 139,
  "vote_average": 8.433,
  "vote_count": 26279,
  "budget": 63000000,
  "revenue": 100853753,
  "genres": [
    {
      "id": 18,
      "name": "Drama"
    }
  ],
  "production_companies": [
    {
      "id": 508,
      "name": "Regency Enterprises"
    }
  ]
}
```

## Authentication

TMDB API uses API key authentication. There are two methods to authenticate your requests:

### Method 1: Query Parameter (Recommended for v3)

Include your API key as a query parameter in every request:

```bash
https://api.themoviedb.org/3/movie/popular?api_key=YOUR_API_KEY
```

### Method 2: Bearer Token (Works with v3 and v4)

Include your access token in the Authorization header:

```bash
curl --request GET \
  --url 'https://api.themoviedb.org/3/movie/popular' \
  --header 'Authorization: Bearer YOUR_ACCESS_TOKEN' \
  --header 'accept: application/json'
```

### Getting Your API Key

1. Create a free account at [TMDB](https://www.themoviedb.org/signup)
2. Go to your [API settings](https://www.themoviedb.org/settings/api)
3. Request an API key and agree to the terms of use
4. Use the provided API key in your requests

**Required Headers:**

- `accept: application/json` - Specify JSON response format
- `Authorization: Bearer {token}` - If using Bearer token method

## Error Handling

The TMDB API returns standardized HTTP status codes and error messages:

### Common HTTP Status Codes

- **200** - Success
- **401** - Authentication failed (Invalid API key)
- **404** - Resource not found
- **422** - Invalid parameters
- **429** - Rate limit exceeded
- **500** - Internal server error
- **503** - Service temporarily offline

### Error Response Format

```json
{
  "status_code": 7,
  "status_message": "Invalid API key: You must be granted a valid key.",
  "success": false
}
```

### Common Errors and Solutions

| Error Code | Status | Description | Solution |
|------------|--------|-------------|----------|
| 7 | 401 | Invalid API key | Verify your API key is correct and active |
| 22 | 400 | Invalid page | Pages start at 1 and max at 500 |
| 25 | 429 | Rate limit exceeded | Reduce request frequency |
| 34 | 404 | Resource not found | Check the resource ID exists |

### Error Handling Best Practices

```javascript
try {
  const response = await fetch(`https://api.themoviedb.org/3/movie/popular?api_key=${API_KEY}`);
  
  if (!response.ok) {
    const error = await response.json();
    throw new Error(`TMDB API Error: ${error.status_message}`);
  }
  
  const data = await response.json();
  return data;
} catch (error) {
  console.error('Failed to fetch movies:', error.message);
  // Handle error appropriately
}
```

## Usage Limits and Best Practices

### Rate Limiting

- **Current Limit**: ~50 requests per second
- **Legacy Limit**: The old 40 requests per 10 seconds limit has been disabled
- **Rate Limit Response**: HTTP 429 status code when exceeded
- **Recommendation**: Implement exponential backoff when receiving 429 responses

### Best Practices

#### 1. Efficient Image Handling

```javascript
// Use configuration endpoint to get base URLs
const config = await fetch('/3/configuration');
const imageBaseUrl = config.images.secure_base_url;
const posterSize = 'w500'; // Choose appropriate size
const fullImageUrl = `${imageBaseUrl}${posterSize}${movie.poster_path}`;
```

#### 2. Implement Caching

- Cache API responses to reduce redundant requests
- Use appropriate cache TTL based on data type
- Static data (genres, configuration) can be cached longer

#### 3. Request Optimization

- Use `append_to_response` parameter to combine multiple requests
- Request only needed data fields when possible
- Implement pagination properly for large datasets

#### 4. Error Handling

- Always handle network timeouts and API errors gracefully
- Implement retry logic with exponential backoff
- Provide fallback options for missing data

#### 5. Respect the Service

- Don't make unnecessary parallel requests
- Use reasonable timeouts for requests
- Monitor your usage and stay within limits

### Example Implementation

```javascript
class TMDBService {
  constructor(apiKey) {
    this.apiKey = apiKey;
    this.baseUrl = 'https://api.themoviedb.org/3';
    this.requestQueue = [];
    this.rateLimit = 50; // requests per second
  }

  async makeRequest(endpoint, params = {}) {
    const url = new URL(`${this.baseUrl}${endpoint}`);
    url.searchParams.append('api_key', this.apiKey);
    
    Object.entries(params).forEach(([key, value]) => {
      url.searchParams.append(key, value);
    });

    try {
      const response = await fetch(url);
      
      if (response.status === 429) {
        // Handle rate limiting
        await this.waitAndRetry();
        return this.makeRequest(endpoint, params);
      }
      
      if (!response.ok) {
        throw new Error(`HTTP ${response.status}: ${response.statusText}`);
      }
      
      return await response.json();
    } catch (error) {
      console.error('TMDB API request failed:', error);
      throw error;
    }
  }

  async waitAndRetry() {
    const delay = Math.pow(2, this.retryCount) * 1000;
    await new Promise(resolve => setTimeout(resolve, delay));
  }
}
```
