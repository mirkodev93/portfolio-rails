# Portfolio Rails Application

A modern portfolio and blog management system built with Ruby on Rails API backend and React/Redux frontend.

## 🚀 Features

- **Portfolio Management**: Showcase your projects with rich content and images
- **Blog System**: Create and manage blog posts with markdown support
- **Content Management System (CMS)**: Admin interface for content management
- **Responsive Design**: Mobile-first approach with modern UI/UX
- **Image Upload**: Support for multiple image formats with cloud storage
- **Tagging System**: Organize content with flexible tagging
- **SEO Optimized**: Built-in SEO features for better search engine visibility

## 🛠 Technology Stack

### Backend
- **Ruby on Rails** - API framework
- **PostgreSQL** - Database
- **Devise** - Authentication
- **CarrierWave** - File uploads
- **RSpec** - Testing framework

### Frontend
- **React** - UI library
- **Redux** - State management
- **Material-UI** - Component library
- **CSS Modules** - Styling
- **Webpack** - Build tool

### Infrastructure
- **CircleCI** - Continuous Integration
- **Code Climate** - Code quality monitoring
- **Capistrano** - Deployment automation

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Ruby (2.7+)
- Rails (6.0+)
- PostgreSQL
- Node.js (14+)
- Yarn or npm

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/mirkodev93/portfolio-rails.git
cd portfolio
```

### 2. Setup the Application
```bash
# Install Ruby dependencies
bundle install

# Install Node.js dependencies
cd frontend
npm install
cd ..

# Setup database
rails db:create
rails db:migrate
rails db:seed

# Start the application
foreman start
```

### 3. Access the Application
- **Client Frontend**: http://localhost:3000
- **CMS Admin**: http://localhost:3000/cms
- **API Documentation**: http://localhost:3000/api/v1

## 📁 Project Structure

```
portfolio-rails/
├── app/                    # Rails application code
│   ├── controllers/        # API controllers
│   ├── models/            # ActiveRecord models
│   ├── serializers/       # JSON serializers
│   └── uploaders/         # File upload handlers
├── frontend/              # React/Redux frontend
│   ├── src/
│   │   ├── client/        # Public-facing React app
│   │   ├── cms/           # Admin CMS React app
│   │   └── shared/        # Shared components and utilities
│   └── webpack.config.js  # Webpack configuration
├── spec/                  # RSpec test files
└── config/                # Rails configuration
```

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the root directory:

```env
DATABASE_URL=postgresql://localhost/portfolio_development
SECRET_KEY_BASE=your_secret_key_here
DEVISE_SECRET_KEY=your_devise_secret_here
```

### Database Configuration
The application uses PostgreSQL. Configure your database settings in `config/database.yml`.

## 🧪 Testing

### Backend Tests
```bash
# Run all RSpec tests
bundle exec rspec

# Run specific test file
bundle exec rspec spec/models/post_spec.rb

# Run tests with coverage
COVERAGE=true bundle exec rspec
```

### Frontend Tests
```bash
cd frontend
npm test
```

## 📚 API Documentation

### Authentication
The API uses token-based authentication with Devise.

### Endpoints

#### Posts
- `GET /api/v1/posts` - List all posts
- `GET /api/v1/posts/:id` - Get a specific post
- `POST /api/v1/posts` - Create a new post (admin only)
- `PUT /api/v1/posts/:id` - Update a post (admin only)
- `DELETE /api/v1/posts/:id` - Delete a post (admin only)

#### Projects
- `GET /api/v1/projects` - List all projects
- `GET /api/v1/projects/:id` - Get a specific project
- `POST /api/v1/projects` - Create a new project (admin only)
- `PUT /api/v1/projects/:id` - Update a project (admin only)
- `DELETE /api/v1/projects/:id` - Delete a project (admin only)

## 🚀 Deployment

### Production Deployment
```bash
# Deploy to production
bundle exec cap production deploy

# Deploy to staging
bundle exec cap staging deploy
```

### Environment Setup
1. Configure your production environment variables
2. Set up your PostgreSQL database
3. Configure your web server (Nginx/Apache)
4. Set up SSL certificates

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Code Style
This project follows the following style guides:
- [Ruby Style Guide](https://github.com/airbnb/ruby)
- [Rails Style Guide](https://github.com/thoughtbot/guides/tree/master/style/rails)
- [JavaScript Style Guide](https://github.com/airbnb/javascript)
- [React Style Guide](https://github.com/airbnb/javascript/tree/master/react)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/tsurupin/portfolio/issues) page
2. Create a new issue with detailed information
3. Include steps to reproduce the problem

## 🔮 Roadmap

- [ ] Upgrade to Rails 7
- [ ] Add real-time features with ActionCable
- [ ] Implement advanced search functionality
- [ ] Add analytics dashboard
- [ ] Support for multiple languages
- [ ] Enhanced SEO features
- [ ] Performance optimizations

## 🙏 Acknowledgments

- Built with [Ruby on Rails](https://rubyonrails.org/)
- Frontend powered by [React](https://reactjs.org/) and [Redux](https://redux.js.org/)
- UI components from [Material-UI](https://material-ui.com/)
- Testing with [RSpec](https://rspec.info/)

---

**Happy Coding! 🎉**