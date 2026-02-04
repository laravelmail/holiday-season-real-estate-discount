# Holiday Season Real Estate Discount

Professional holiday season real estate marketing email promoting discounts and deals

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Real Estate
- **Message Type:** Marketing
- **Tags:** promotion, discount, holiday season

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/holiday-season-real-estate-discount.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/holiday-season-real-estate-discount/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.holiday-season-real-estate-discount',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
