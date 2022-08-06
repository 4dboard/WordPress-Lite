![image](https://user-images.githubusercontent.com/6468571/183256208-c68f8f50-d0fd-4dde-85ad-7e2ea828f78e.png)

# WordPress Lite (Project)
## WordPress has become more powerful, faster and more compact, introducing the WordPress Lite Project. 

This project's goal is to build a version of WordPress that is both as efficient and as space-saving as is reasonably possible. This will be accomplished by combining several server projects into a single reliable application. A variety of server projects will be combined in order to attain this goal. This will be done so that the objective that has been established for the project may be accomplished.

![image](https://user-images.githubusercontent.com/6468571/183256289-47223674-67ef-4064-8c4b-09a1bbd97981.png)

Because WordPress Lite is plug-and-play, no database configuration or installation is required. This is because no installation needs are necessary. WordPress Lite is a much more efficient and space-saving version of WordPress. Here, WordPress Lite is available for free download. It is not essential to update the database or install additional software; it is sufficient to just add it. Compatible with more recent PHP versions than version 7.2. Compatible with future releases and implementation-ready Due to the fact that adding public dependencies to a project adds just a little amount of new data, the file storage requirements for tracking many versions of your work are surprisingly low. This is the case since adding public dependents offers minimal more data.

![image](https://user-images.githubusercontent.com/6468571/183256576-c1024d67-7bb7-4798-ab6f-8bbbacf430b7.png)

<hr/>

## Features

- "Plug and Play," no installation required. 

- No Database or Database Configuration required.

- Optimized for Maximum Efficiency and Performance.

- 90% more small and more efficient than legacy WordPRess.

- Support for the WPackagist Repository and the Composer Repository.

- True version control with Git and GitHub.

- Compatible with PHP versions 7.2 and above.

- Deployment friendly with Environment Variables.

![image](https://user-images.githubusercontent.com/6468571/183256359-59495c98-c5a8-4a9a-b79f-5d1bab7ce213.png)

WordPress Lite uses the Roots.io's Bedrock framework employs composer dependencies to facilitate WordPress installation. This not only makes it simpler for our team to manage ".env" files, but also allows us to create a centralized and carefully controlled staging environment. Websites that deviate from normal file path patterns may be resistant to automated assaults and security issues. The reason for this is that file paths provide a security risk. Utilizing non-standard file paths might potentially improve security and protection. These additional delights are entirely optional. 

![image](https://user-images.githubusercontent.com/6468571/183256546-9e3ae3ca-a114-4b3b-ad72-072af4374ed3.png)

Using public dependencies adds a negligible amount of files to a project; hence, the real file storage needs for monitoring several versions of your work are rather modest. Therefore, the real file storage needs for maintaining several versions of a work are minimal. This is because there are presently few loaded files in the project. It is possible to put the whole Bedrock directory under version control to guarantee that a large number of developers adhere to the same plugin and other standards. Consequently, it is now feasible. WordPress in its most basic form cannot do this alone.

![image](https://user-images.githubusercontent.com/6468571/183256500-cfc3c37a-ade0-4e89-a2bf-0c3a4664be5a.png)

<hr/>

<p align="center">
  <a href="LICENSE.md">
    <img alt="MIT License" src="https://img.shields.io/github/license/roots/bedrock?color=%23525ddc&style=flat-square" />
  </a>

  <a href="https://packagist.org/packages/roots/bedrock">
    <img alt="Packagist" src="https://img.shields.io/packagist/v/roots/bedrock.svg?style=flat-square" />
  </a>

  <a href="https://github.com/roots/bedrock/actions/workflows/ci.yml">
    <img alt="Build Status" src="https://img.shields.io/github/workflow/status/roots/bedrock/CI?style=flat-square" />
  </a>

  <a href="https://twitter.com/rootswp">
    <img alt="Follow Roots" src="https://img.shields.io/twitter/follow/rootswp.svg?style=flat-square&color=1da1f2" />
  </a>
</p>

<p align="center">
  <a href="https://roots.io/bedrock/">
    <img alt="Bedrock" src="https://cdn.roots.io/app/uploads/logo-bedrock.svg" height="100">
  </a>
</p>

<h2 align="center">A modern WordPress stack</h2>

<p align="center">
  <a href="https://roots.io/"><strong><code>Website</code></strong></a> &nbsp;&nbsp; <a href="https://docs.roots.io/bedrock/master/installation/"><strong><code>Documentation</code></strong></a> &nbsp;&nbsp; <a href="https://github.com/roots/bedrock/releases"><strong><code>Releases</code></strong></a> &nbsp;&nbsp; <a href="https://discourse.roots.io/"><strong><code>Support</code></strong></a>
</p>

<hr/>

## Overview

Bedrock is a modern WordPress stack that helps you get started with the best development tools and project structure.

Much of the philosophy behind Bedrock is inspired by the [Twelve-Factor App](http://12factor.net/) methodology including the [WordPress specific version](https://roots.io/twelve-factor-wordpress/).

![image](https://user-images.githubusercontent.com/6468571/183256466-c0c16d32-1944-46d1-abb3-80e2487e5c6b.png)

<hr/>

## Features

- Better folder structure
- Dependency management with [Composer](https://getcomposer.org)
- Easy WordPress configuration with environment specific files
- Environment variables with [Dotenv](https://github.com/vlucas/phpdotenv)
- Autoloader for mu-plugins (use regular plugins as mu-plugins)
- Enhanced security (separated web root and secure passwords with [wp-password-bcrypt](https://github.com/roots/wp-password-bcrypt))

![image](https://user-images.githubusercontent.com/6468571/183256454-4fffe2aa-9b3c-48da-b976-7c92857e7888.png)

<hr/>

## Requirements

- PHP >= 7.4
- Composer - [Install](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

<hr/>

## Installation

1. Create a new project:
   ```sh
   $ composer create-project roots/bedrock
   ```
   By default, this installs the `dist` version of all dependent packages.  To install the `source` versions instead, update `composer.json` as follows:
   ```json
    "preferred-install": {
      "roots/wordpress-no-content": "dist",
      "*": "source"
    },
   ```
2. Update environment variables in the `.env` file. Wrap values that may contain non-alphanumeric characters with quotes, or they may be incorrectly parsed.

- Database variables
  - `DB_NAME` - Database name
  - `DB_USER` - Database user
  - `DB_PASSWORD` - Database password
  - `DB_HOST` - Database host
  - Optionally, you can define `DATABASE_URL` for using a DSN instead of using the variables above (e.g. `mysql://user:password@127.0.0.1:3306/db_name`)
- `WP_ENV` - Set to environment (`development`, `staging`, `production`)
- `WP_HOME` - Full URL to WordPress home (https://example.com)
- `WP_SITEURL` - Full URL to WordPress including subdirectory (https://example.com/wp)
- `AUTH_KEY`, `SECURE_AUTH_KEY`, `LOGGED_IN_KEY`, `NONCE_KEY`, `AUTH_SALT`, `SECURE_AUTH_SALT`, `LOGGED_IN_SALT`, `NONCE_SALT`
  - Generate with [wp-cli-dotenv-command](https://github.com/aaemnnosttv/wp-cli-dotenv-command)
  - Generate with [our WordPress salts generator](https://roots.io/salts.html)

3. Add theme(s) in `web/app/themes/` as you would for a normal WordPress site
4. Set the document root on your webserver to Bedrock's `web` folder: `/path/to/site/web/`
5. Access WordPress admin at `https://example.com/wp/wp-admin/`

<hr/>

## Community

Keep track of development and community news.

- Join us on Discord by [sponsoring us on GitHub](https://github.com/sponsors/roots)
- Participate on the [Roots Discourse](https://discourse.roots.io/)
- Follow [@rootswp on Twitter](https://twitter.com/rootswp)
- Read and subscribe to the [Roots Blog](https://roots.io/blog/)
- Subscribe to the [Roots Newsletter](https://roots.io/subscribe/)
