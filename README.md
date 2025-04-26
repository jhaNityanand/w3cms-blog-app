# W3CMS Blog Application

A modern, feature-rich blog application built with Laravel PHP framework. This application provides a robust platform for creating, managing, and sharing blog content with a beautiful and responsive user interface.

## Features

- 🚀 Built with Laravel 10.x
- 💅 Styled with Tailwind CSS
- 📱 Fully responsive design
- 🔒 Authentication and authorization
- 📝 Rich text editor for blog posts
- 🖼️ Image upload and management
- 🔍 Search functionality
- 📊 Analytics and statistics
- 🌐 SEO optimized

## Prerequisites

Before you begin, ensure you have the following installed:
- PHP (v8.1 or higher)
- Composer
- MySQL (v5.7 or higher)
- Node.js (v18.0.0 or higher) - for frontend assets
- npm (v9.0.0 or higher)
- Git

## Installation

1. Clone the repository:
```bash
git clone https://github.com/jhaNityanand/w3cms-blog-app.git
cd w3cms-blog-app
```

2. Install PHP dependencies:
```bash
composer install
```

3. Install frontend dependencies:
```bash
npm install
```

4. Create a `.env` file by copying `.env.example`:
```bash
cp .env.example .env
```

5. Generate application key:
```bash
php artisan key:generate
```

6. Configure your database in `.env` file:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password
```

7. Run database migrations:
```bash
php artisan migrate
```

8. Start the development server:
```bash
php artisan serve
```

9. In a separate terminal, compile frontend assets:
```bash
npm run dev
```

The application will be available at `http://localhost:8000`

## Project Structure

```
w3cms-blog-app/
├── app/                 # Application core code
│   ├── Http/           # Controllers, Middleware, Requests
│   ├── Models/         # Eloquent models
│   └── Services/       # Business logic services
├── config/             # Configuration files
├── database/           # Database migrations and seeders
├── public/             # Publicly accessible files
├── resources/          # Views, assets, and language files
│   ├── js/            # JavaScript files
│   ├── css/           # CSS files
│   └── views/         # Blade templates
├── routes/             # Route definitions
└── storage/            # Application storage
```

## Available Commands

- `php artisan serve` - Start the development server
- `php artisan migrate` - Run database migrations
- `php artisan migrate:fresh --seed` - Reset database and run seeders
- `php artisan make:model ModelName -mcr` - Create model with migration and controller
- `php artisan route:list` - List all registered routes
- `php artisan cache:clear` - Clear application cache
- `npm run dev` - Compile frontend assets for development
- `npm run build` - Compile frontend assets for production

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please open an issue in the GitHub repository or contact the maintainers.

## Acknowledgments

- Laravel team for the amazing framework
- Tailwind CSS for the utility-first CSS framework
- All contributors who have helped shape this project
