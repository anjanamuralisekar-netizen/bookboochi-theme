=== Bookboochi ===
Contributors: anjanamuralisekar
Requires at least: 6.4
Tested up to: 6.6
Requires PHP: 7.4
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html
Tags: blog, one-column, right-sidebar, custom-logo, custom-menu, featured-images, threaded-comments, translation-ready, accessibility-ready

A warm, literary WordPress theme built for Bookboochi — a book review and
reading blog — hand-coded (no page builder dependency) for speed and for
SEO / AEO / GEO (Answer & Generative Engine Optimization).
Website: bookboochi.site

== Description ==

Bookboochi is a classic PHP theme. There is no drag-and-drop builder to
learn: write posts in the normal WordPress editor, fill in the optional
"Book Review Details" box on any post, and the theme takes care of layout,
schema markup, and machine-readability.

= What "SEO / AEO / GEO optimized" means in this theme =

* SEO (search engines): title/meta description control per post, canonical
  URLs, Open Graph + Twitter Card tags, semantic HTML5, fast/lean markup
  (no jQuery dependency, deferred scripts, no emoji-script bloat), the
  built-in WordPress XML sitemap left enabled, and a robots.txt that adds
  your sitemap.
* AEO (answer engines like Google's featured snippets / voice assistants):
  an optional on-page FAQ block with matching FAQPage schema, a "TL;DR"
  shortcode for a short quotable answer near the top of a post, and an
  auto-generated table of contents with anchor links for long posts.
* GEO (generative engines — ChatGPT, Perplexity, Google AI Overviews,
  Claude, etc.): rich JSON-LD (Organization, WebSite, BreadcrumbList,
  BlogPosting, Book, Review, Person/author, FAQPage), an author bio box on
  every post for E-E-A-T (experience/expertise/authority/trust) signal, a
  `/llms.txt` endpoint summarizing the site for LLM crawlers, and a
  robots.txt that explicitly allows well-known AI crawlers instead of
  silently blocking them.

= Book review layout =

Open any post's editor and scroll to the "Book Review Details" box. Fill
in the book title (required to activate the box) plus any of: author,
genre, publisher, ISBN, pages, your 0–5 rating, a one-line verdict, and a
buy/find link. Save the post and a structured "Book at a glance" box
appears above the comments, with matching Book + Review schema in the
page's JSON-LD.

== Installation ==

1. In WordPress admin, go to Appearance → Themes → Add New → Upload Theme.
2. Choose the bookboochi.zip file and click Install Now, then Activate.
3. Go to Appearance → Menus and assign a menu to "Primary Menu" (and
   optionally "Footer Menu").
4. Go to Appearance → Customize → Bookboochi Colors / Social Links /
   Footer to set your accent color and social links.
5. Go to Settings → General and confirm your Tagline — it feeds the
   site's meta description and JSON-LD description.
6. Go to Settings → Permalinks and click Save (this activates the
   `/llms.txt` route cleanly).

== Frequently asked questions ==

= Do I need any plugins? =

No — SEO meta tags, Open Graph tags, and JSON-LD schema are all built in.
If you later install Yoast SEO, Rank Math, or All in One SEO, this theme
automatically stops outputting its own meta tags so nothing conflicts.

= Where do I set a custom SEO title or meta description for a post? =

Open the post editor and scroll down to the "Bookboochi SEO / Social" box
below the content editor.

== Changelog ==

= 1.0.5 =
* Fix: the "Find this book" button (and any other .bb-btn) showed
  low-contrast dark text instead of white once a browser considered its
  link visited, due to a CSS specificity conflict.

= 1.0.4 =
* Fix: a menu item with sub-items (e.g. a "Genre" parent listing every
  genre) rendered its children inline instead of as a dropdown. Nested
  menu items now open as a proper dropdown on desktop (hover, keyboard
  focus, or tap on touchscreens) and as an indented stacked list on
  mobile.

= 1.0.3 =
* The "Book at a glance" box now appears above the review text (right
  after the featured image) instead of below it.

= 1.0.2 =
* The "Book at a glance" box's Author and Genre now link to their
  archive pages when a post is also tagged with the Bookboochi Library
  plugin's Author/Genre taxonomies — previously always plain text.

= 1.0.1 =
* Fix: custom taxonomy archive pages (e.g. Book Genre / Book Author pages
  added by the Bookboochi Library plugin) showed a literal "<span>" tag
  in the breadcrumb instead of rendering it.

= 1.0.0 =
* Initial release.

== Credits ==

* Fonts: Playfair Display, Source Serif 4, and Inter (Google Fonts,
  SIL Open Font License).
* Theme code is licensed GPLv2 or later, same as WordPress itself.
