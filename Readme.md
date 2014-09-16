Codeigniter SEO Helper
=======================
Generates Meta tags for description, open graph, Twitter & also robots
-----------------------

## Installation

**Step 1**
Place the files inside config and helpers into the corresponding folders of your CI application.
Files:
1. config/seo_config
2. helpers/seo_helper

**Step 2**
1. Open autoload.php inside of your config folder 
2. Add seo_helper to the autoload helper

**Step 3**
1. Open up seo_helper you copied earlier
2. Change the title, description and image URL to anything you like.
(Note: Description maximum 155 characters)

```php
$autoload['helper'] = array('url','seo_helper');
```

## Usage
It's very easy to use, just go to any view files of your application and include this line:
```php
meta_tags();
```

When your page is loaded, the meta tags will be injected automactically



