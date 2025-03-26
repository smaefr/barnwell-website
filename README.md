# Barnwell Website

A responsive single-page website for Barnwell, a jumper barn located in Nassau County, Florida. The site showcases the facility, horses, team members, and includes a blog section called "Scary Corner."

## Features

- Responsive design that works across all device sizes
- Interactive horse profiles with image galleries
- Team member showcase
- Integrated blog system with search functionality
- Lightbox image viewer for horse photos
- Custom navigation system
- Mobile-friendly interface

## Technologies Used

- HTML5
- CSS3 (with custom styling and animations)
- JavaScript (ES6+)
- jQuery
- SASS/SCSS for styling
- External APIs for blog functionality

## Project Structure

```
barnwell/
├── assets/
│   ├── css/
│   │   └── main.css
│   ├── js/
│   │   ├── browser.min.js
│   │   ├── breakpoints.min.js
│   │   ├── jquery.min.js
│   │   ├── main.js
│   │   └── util.js
│   └── sass/
│       └── libs/
│           ├── _functions.scss
│           └── _vendor.scss
├── images/
│   ├── attoranta/
│   ├── ruby/
│   ├── titania/
│   ├── barnwell-top.png
│   ├── barnwell-bottom.png
│   └── background.png
└── index.html
```

## Setup and Installation

1. Clone the repository:
```bash
git clone https://github.com/smaefr/barnwell-website.git
```

2. Navigate to the project directory:
```bash
cd barnwell-website
```

3. Open `index.html` in a web browser to view the site locally.

## Development

To modify the styles:

1. Install SASS if you haven't already:
```bash
npm install -g sass
```

2. Watch for SASS changes:
```bash
sass --watch assets/sass:assets/css
```

## API Integration

The blog functionality uses a custom API endpoint:
- Base URL: `https://barnwell-blog-worker.admtech.us/api/blog`
- Available endpoints:
  - `GET ?action=get_posts` - Retrieve all blog posts
  - `GET ?action=get_post&slug={slug}` - Retrieve a specific post
  - `GET ?action=get_posts&search={term}` - Search posts

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Security Considerations

- All external resources are loaded over HTTPS
- Input sanitization is implemented for blog search
- API requests are properly validated

## Performance Optimizations

- Lazy loading for images
- Minified JavaScript and CSS
- Optimized image assets
- Efficient DOM manipulation

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is proprietary and maintained by ADM Technology. All rights reserved.

## Credits

- Website development by [ADM Technology](https://admtech.org)
- Horse photography provided by Barnwell
- Icons and design elements: [Attribution if applicable]

## Contact

For questions or support, please contact:
- Website maintenance: [ADM Technology](https://admtech.org)
