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

Example:

```php
$autoload['helper'] = array(,'seo_helper');
```

## Usages
It's very easy to use, just go to any view files of your application and include this line:
```php
meta_tags();
```

When your page is loaded, the meta tags will be injected automactically

##Customizations

Controlling which meta tags should be injected

Types of Meta Tags included:
  * Description
  * Og (Open graph)
  * Twitter
  * Robot

```php
$e = array(
	'general' => true, //description
	'og' => true,
	'twitter'=> true,
	'robot'=> true
);
meta_tags($e, $title = '', $desc = '', $imgurl ='', $url = '');
```
Just change the true to false to disable them.
You can also customize the title, desc, image url and url for certain pages.

**NOTE: If title, desc, image url and url are left empty, it will use the default ones set inside config file.**

#Follow me on Twtter [@elsodev](http://twitter.com/elsodev)



