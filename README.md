# kitloom — start from WordPress, grow on Laravel, run it with AI

**Start from WordPress. Grow on Laravel. Run it with AI.** Bring the WordPress site you have — kitloom runs on its database as it is: posts, pages, meta, options, users, menus, media, comments, the plugins' data, the same URLs and permalinks, with no export, import or URL rewrite. Or start a new site on the same data model, with no WordPress installed. Either way, Claude, Cursor or your own AI agent does the site's work through a built-in MCP server, with exactly the rights of the user whose key it holds: drafts for an author's key, locked settings, nothing deleted for good, every change in the activity log. The admin is [Filament](#kitloom-for-filament) or [Laravel Nova](#kitloom-for-nova); the front end is Blade, Vue, React or plain JSON.

This repository is where kitloom users and the people evaluating it talk to us: questions, ideas and bug reports. The product's code is not here — it is installed with Composer from the kitloom package repository after purchase.

## Try it

- **Live demo, no sign-up:** your own [Filament sandbox](https://filament.kitloom.dev/new) or [Nova sandbox](https://nova.kitloom.dev/new) in one click, with every module and theme.
- [Documentation](https://kitloom.dev/docs/introduction.html) · [Installation](https://kitloom.dev/docs/installation.html) · [Migrate from WordPress](https://kitloom.dev/docs/migrate-from-wordpress.html) · [Changelog](https://kitloom.dev/docs/changelog.html)
- [Pricing](https://kitloom.dev/pricing.html): Kitloom for Filament or Kitloom for Nova, one site or unlimited, 14-day refund without questions.

## What you get

- **A WordPress-compatible core on Laravel 13**: the request handled the way WordPress does it — rewrite rules, the main query, the template hierarchy, shortcodes, widgets and dynamic blocks — with Eloquent models over the WordPress tables.
- **40+ modules**, each a Composer package that plugs itself in: SEO, redirects and a 404 monitor, contact forms, custom fields, custom post types, a shop, bookings, online courses, real estate listings, languages, backups, a link checker, cookie consent, analytics and tag manager, two-factor authentication, social login, webhooks, the WordPress REST API and more — see the [module catalog](https://kitloom.dev/docs/modules/catalog.html).
- **Themes in Blade, Vue or React** (Inertia), 14 bundled ones with demo content, and `php artisan kitloom:make-theme` to generate your own — see the [theme catalog](https://kitloom.dev/docs/themes/catalog.html).
- **A headless CMS when you want one**: every page also answers as JSON, next to the WordPress REST API (`/wp-json/wp/v2`).
- **AI agents over MCP**: Claude, Cursor or your own agent connects to the site's `/mcp` and runs it — posts, media, SEO, redirects, menus, the shop's orders — with the rights of the user whose key it holds; nothing is deleted for good. See [AI Agents](https://kitloom.dev/docs/ai.html) and [Two Ways to Use AI](https://kitloom.dev/docs/ai-overview.html).

## WordPress plugins whose data it reads

kitloom reads the tables and meta these plugins leave behind, so their content comes along without an export:

| Area | WordPress plugin |
|---|---|
| Shop | WooCommerce (HPOS) |
| Custom fields, post types and taxonomies | Advanced Custom Fields (ACF), Secure Custom Fields |
| Forms and messages | Contact Form 7, Flamingo |
| SEO, redirects, 404 monitor, internal links | Rank Math |
| Languages | Polylang, WPML (converted) |
| Courses | LearnPress |
| Listings | Houzez, Listeo |
| Sliders | Slide Anything |
| Social login | Nextend Social Login |

## Kitloom for Filament

The whole admin in [Filament](https://filamentphp.com) 5, at `/admin`: posts and pages with a visual editor and their translations, the media library over WordPress attachments, menus, widgets and themes, custom fields, users and roles, every WordPress settings screen, and a section per module. Modules are switched on and off on the Modules screen. After purchase, a new site starts with:

```bash
composer create-project kitloom/filament-skeleton my-site --repository=https://packages.kitloom.dev --add-repository
```

## Kitloom for Nova

The same admin in [Laravel Nova](https://nova.laravel.com) 5, at `/nova`, with every module's section. Nova is sold by Laravel, not with kitloom: every site needs its own Nova license. A new site starts with:

```bash
composer create-project kitloom/nova-skeleton my-site --repository=https://packages.kitloom.dev --add-repository
```

Either edition fits into an existing Laravel 13 application too — see [Installation](https://kitloom.dev/docs/installation.html). Requirements: PHP 8.4+, Laravel 13, MySQL (a WordPress database or an empty one) or SQLite.

## Who it is for

Teams with a WordPress site that has outgrown its plugins and want Laravel — queues, tests, Eloquent, their own code — without rewriting the content, the URLs or the editors' habits. If you want a Laravel CMS with no WordPress in it at all, kitloom is not that: its data is in WordPress's shape on purpose. More in [WordPress and Laravel](https://kitloom.dev/docs/wordpress-and-laravel.html).

## Where to write

| You want to… | Go to |
|---|---|
| ask how to do something, or whether kitloom fits your site | [Discussions → Q&A](https://github.com/kitloom/kitloom/discussions/categories/q-a) |
| suggest a feature, a module or a WordPress plugin to cover | [Discussions → Ideas](https://github.com/kitloom/kitloom/discussions/categories/ideas) |
| report a bug | [Issues → New issue](https://github.com/kitloom/kitloom/issues/new/choose) |
| report a security vulnerability | **privately**, see [SECURITY.md](https://github.com/kitloom/kitloom/blob/main/SECURITY.md) |
| ask about a purchase, a license or a refund | support@kitloom.dev |

We read everything here and answer within a business day.

---

This repository's `composer.json` only describes kitloom for Packagist: requiring `kitloom/kitloom` installs nothing of kitloom itself.
