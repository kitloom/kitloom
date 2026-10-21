# kitloom

**A Laravel CMS for sites with WordPress data.** Move a WordPress site to Laravel with its database as it is: every post, option and URL comes along. Filament or Nova is the admin; Blade, Vue, React or plain JSON the front; MCP gives your AI agent exactly the access you decide.

This repository is where kitloom users and the people evaluating it talk to us. The product's code is not here: it is installed with Composer from the kitloom package repository after purchase.

## Try it

- [Filament demo](https://filament.kitloom.dev/new) and [Nova demo](https://nova.kitloom.dev/new): your own sandbox in one click, no sign-up.
- [Documentation](https://kitloom.dev/docs/introduction.html) · [Installation](https://kitloom.dev/docs/installation.html) · [Migrate from WordPress](https://kitloom.dev/docs/migrate-from-wordpress.html)
- [Pricing](https://kitloom.dev/pricing.html): Filament Edition and Nova Edition, 14-day refund without questions.
- [Changelog](https://kitloom.dev/docs/changelog.html)

## The Nova Edition

The whole admin drawn in Laravel Nova 5, at `/nova`: posts and pages with a visual editor and their translations, the media library over WordPress attachments, menus, widgets and themes, custom fields on ACF's data model, users and roles, every WordPress settings screen, and a section per module — SEO, redirects, forms, a shop, bookings, courses, listings, backups, languages, the MCP server for AI agents and more. Each module is a Composer package that plugs itself in and can be switched off on the Modules screen.

Nova is sold by Laravel, not with kitloom: every site needs its own [Nova license](https://nova.laravel.com). After purchase, a new site starts with:

```bash
composer create-project kitloom/nova-skeleton my-site --repository=https://packages.kitloom.dev --add-repository
```

An existing Laravel 13 application with Nova 5 adds the packages instead — see [Installation](https://kitloom.dev/docs/installation.html). This repository's `composer.json` only describes kitloom for Packagist: requiring `kitloom/kitloom` installs nothing of kitloom itself.

## Where to write

| You want to… | Go to |
|---|---|
| ask how to do something, or whether kitloom fits your site | [Discussions → Q&A](../../discussions/categories/q-a) |
| suggest a feature, a module or a WordPress plugin to cover | [Discussions → Ideas](../../discussions/categories/ideas) |
| report a bug | [Issues → New issue](../../issues/new/choose) |
| report a security vulnerability | **privately**, see [SECURITY.md](SECURITY.md) |
| ask about a purchase, a licence or a refund | support@kitloom.dev |

We read everything here and answer within a business day.
