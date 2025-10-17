# CAPTCHA Solver Application Frontend

This project provides a simple, single-file responsive web application designed to help users solve CAPTCHAs. It defaults to a provided sample image but can also load CAPTCHA images from a URL parameter.

## Features

-   **Responsive Design:** Built with Tailwind CSS, ensuring a consistent look and feel across various devices.
-   **Dynamic Image Loading:** Displays a CAPTCHA image either from the attached `sample.png` or a specified URL.
-   **User Input:** Provides an input field for users to type the CAPTCHA text.
-   **Basic Validation:** For the default `sample.png`, it checks if the entered text matches the hardcoded solution. For external URLs, it provides a prompt as automatic verification would require a backend or advanced OCR capabilities not included in this simple frontend app.
-   **Single File:** All HTML, CSS (via Tailwind CDN), and JavaScript are contained within a single `index.html` file for easy deployment and testing.

## Usage

### Local Setup

1.  Save the `index.html`, `README.md`, `LICENSE`, and `sample.png` files into the same directory.
2.  Open `index.html` in your web browser.

### Default CAPTCHA

When you open `index.html` without any URL parameters, it will display the `sample.png` CAPTCHA image.

### Loading an External CAPTCHA

You can specify an external image URL using the `url` query parameter. For example:

```
index.html?url=https://example.com/some-captcha-image.png
```

When an external URL is used, the application relies on the user to accurately solve the CAPTCHA, as programmatic verification for arbitrary images is outside the scope of this frontend-only application.

## Technologies Used

-   **HTML5:** For the application structure.
-   **Tailwind CSS (CDN):** For styling and responsive layout.
-   **JavaScript:** For dynamic behavior, image loading, and input handling.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.