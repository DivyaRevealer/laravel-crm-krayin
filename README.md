<p align="center">
<a href="http://revealercrm.com"><img src="https://bagisto.com/wp-content/uploads/2021/06/bagisto-logo.png" alt="Total Downloads"></a>
</p>

<p align="center">
<a href="https://packagist.org/packages/revealer/laravel-crm"><img src="https://poser.pugx.org/revealer/laravel-crm/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/revealer/laravel-crm"><img src="https://poser.pugx.org/revealer/laravel-crm/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/revealer/laravel-crm"><img src="https://poser.pugx.org/revealer/laravel-crm/license.svg" alt="License"></a>
</p>


![enter image description here](https://raw.githubusercontent.com/revealer/temp-media/master/dashboard.png)

## Topics

1. [Introduction](#introduction)
2. [Documentation](#documentation)
3. [Requirements](#requirements)
4. [Installation & Configuration](#installation-and-configuration)
4. [Docker Installation](https://devdocs.revealercrm.com/2.0/introduction/docker.html)
5. [License](#license)
6. [Security Vulnerabilities](#security-vulnerabilities)

### Introduction

[Revealer CRM](https://revealercrm.com) is a hand tailored CRM framework built on some of the hottest opensource technologies
such as [Laravel](https://laravel.com) (a [PHP](https://secure.php.net/) framework) and [Vue.js](https://vuejs.org)
a progressive Javascript framework.

**Free & Opensource Laravel CRM solution for SMEs and Enterprises for complete customer lifecycle management.**

**Read our documentation: [Revealer CRM Docs](https://devdocs.revealercrm.com/)**

**We also have a forum for any type of concerns, feature requests, or discussions. Please visit: [Revealer CRM Forums](https://forums.revealercrm.com/)**

# Visit our live [Demo](https://demo.revealercrm.com)

<a href="javascript:void();">
     <img class="flag-img" src="https://raw.githubusercontent.com/revealer/temp-media/master/visit-our-live-demo.png" alt="Chinese" width="100%">
</a>

It packs in lots of features that will allow your E-Commerce business to scale in no time:

-   Descriptive and Simple Admin Panel.
-   Admin Dashboard.
-   Custom Attributes.
-   Built on Modular Approach.
-   Email parsing via Sendgrid.
-   Check out [these features and more](https://revealercrm.com/features/).
  
**For Developers**:
Take advantage of two of the hottest frameworks used in this project -- Laravel and Vue.js -- both of which have been used in Revealer CRM.

### Documentation

#### Revealer Documentation [https://devdocs.revealercrm.com](https://devdocs.revealercrm.com)

### Requirements

-   **SERVER**: Apache 2 or NGINX.
-   **RAM**: 3 GB or higher.
-   **PHP**: 8.1 or higher
-   **For MySQL users**: 5.7.23 or higher.
-   **For MariaDB users**: 10.2.7 or Higher.
-   **Node**: 8.11.3 LTS or higher.
-   **Composer**: 2.5 or higher

### Installation and Configuration

##### Execute these commands below, in order

```
composer create-project
```

-   Find **.env** file in root directory and change the **APP_URL** param to your **domain**.

-   Also, Configure the **Mail** and **Database** parameters inside **.env** file.

```
php artisan revealer-crm:install
```

**To execute Revealer**:

##### On server:

Warning: Before going into production mode we recommend you uninstall developer dependencies.
In order to do that, run the command below:

> composer install --no-dev

```
Open the specified entry point in your hosts file in your browser or make an entry in hosts file if not done.
```

##### On local:

```
php artisan route:clear
php artisan serve
```


**How to log in as admin:**

> _http(s)://example.com/admin/login_

```
email:admin@example.com
password:admin123
```

### Customizing the Footer

To change the text shown in the footer or the "Powered by" message:

1. Sign in to your **admin** panel.
2. Navigate to **Settings > Configuration**.
3. Under **General**, open the **Footer** section.
4. Edit the **Powered by** field with your desired text and save.

The value is stored in the `general.settings.footer.label` configuration key, so you can also seed or update it directly if needed.

### WhatsApp CRM Integration

[Revealer CRM WhatsApp](https://revealercrm.com/extensions/revealer-crm-whatsapp-extension/) Extension enables the store administrator to generate leads via their WhatsApp number.

![enter image description here](https://raw.githubusercontent.com/revealer/temp-media/master/revealer-crm-whatsapp-integration.png)

### VoIP CRM Integration

[Revealer CRM VoIP](https://revealercrm.com/extensions/revealer-crm-voip/) extension allows the user to make Trunk calls over a broadband Internet connection and the user can also perform Inbound routes.

![enter image description here](https://raw.githubusercontent.com/revealer/temp-media/master/revealer-voip.png)

### Building Admin Assets

If you add new images or change static files in the admin area, rebuild the assets so the updates appear in `public/admin/build`.

1. `cd packages/Webkul/Admin`
2. Run `npm install` to install Node dependencies.
3. Execute `npm run build` to compile the assets.
4. Commit the generated `public/admin/build` files to Git.
   
### License

Revealer CRM is a fully open-source CRM framework which will always be free under the [MIT License](https://github.com/revealer/laravel-crm/blob/2.1/LICENSE).

### Security Vulnerabilities

Please don't disclose security vulnerabilities publicly. If you find any security vulnerability in Revealer CRM then please email us: sales@revealercrm.com.
