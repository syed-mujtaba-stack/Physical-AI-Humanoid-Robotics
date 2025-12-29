# Technical Architecture

## Frontend
- **Framework**: Docusaurus v3 for static site generation
- **Content Format**: MDX (Markdown with JSX) for interactive content
- **Components**: Custom React components for interactive elements
- **Styling**: CSS modules and Docusaurus theme customization
- **Build System**: Webpack-based build pipeline
- **Static Assets**: Optimized images, diagrams, and media files

## Backend
- **Framework**: FastAPI for RAG pipeline and API services
- **Language**: Python for backend logic and processing
- **RAG Pipeline**: Retrieval-Augmented Generation for contextual answers
- **API Endpoints**: RESTful APIs for chatbot integration
- **Authentication**: Better Auth for user management
- **Content Processing**: Text parsing and vectorization services

## Vector Database
- **Provider**: Qdrant Cloud Free Tier
- **Purpose**: Store and retrieve textbook content embeddings
- **Indexing**: Content chunks with metadata for semantic search
- **Search**: Vector similarity search for contextual retrieval
- **Maintenance**: Automated content indexing and updates

## Relational Database
- **Provider**: Neon Serverless Postgres
- **Purpose**: User data, profiles, authentication, and metadata
- **Schema**: User accounts, profiles, preferences, and session data
- **Scaling**: Serverless architecture with automatic scaling
- **Security**: Encrypted connections and data protection

## Deployment
- **Frontend Hosting**: GitHub Pages for static site delivery
- **Backend Hosting**: Vercel or Render for API services
- **CDN**: GitHub Pages CDN for global content delivery
- **Domains**: Custom domain configuration with SSL certificates
- **Monitoring**: Performance and availability tracking

## Content Ingestion Flow
1. **Content Creation**: Authors create MDX content files
2. **Content Parsing**: Text extraction and preprocessing pipeline
3. **Vectorization**: Text chunks converted to embeddings
4. **Indexing**: Embeddings stored in Qdrant Cloud with metadata
5. **Synchronization**: Content updates automatically reflected
6. **Caching**: Optimized caching strategies for performance