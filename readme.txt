=== Real Search - Advanced Search Plugin ===
Contributors: wprealsearch
Tags: search, fulltext search, relevant search, lucene, stemmer, natural language, natural language processing
Requires at least: 3.8
Tested up to: 4.7.3
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.htm

The RealSearch search plugin replaces the default search with a Lucene based one, thus, delivering more accurate and relevant search results.
Search inside attachments, DOCX, XLSX and even images,

== Description ==
The RealSearch WordPress Search Plugin replaces the default MySQL based search with a much more powerful **Lucene** based one, thus, delivering more accurate and relevant search results.

= Features: =

* Keyword lemmatization (stemming): **shoot in feet** is the same as **shot in foot**
* Sorting based on relevancy.
* Search keyword *highlight*.
* Live ajax search with type head or live search.
* Boolean queries: Digital camera **OR** Laptop **AND** water resistant
* Exclude search terms with the ”-” operator: **Install -Windows**
* Fuzzy search: envito~ 0.1, codecanon~ 0.2
* Wildcard search: **Insta\* Window\***
* Search for shortcode content

= Live AJAX Search =

The RealSearch Plugin offers a blazingly fast Live AJAX Search; it achieves this by pre-caching 500 documents, and if the searched keyword does not match any of them, then it will do an AJAX search request.

= Search statistics =

You can monitor search performance by keywords and also observe trends in search and click through volumes in the “Stats” page.

= Info and documentation =
You can find more information at the [Search Plugin Wordpress](http://searchpluginwordpress.com/) blog.

= Plugin requirements =

Requires PHP 5.3.0 (min), PHP 5.4.0 (all) 32 MB RAM (Depends on index size). Search feature has been tested only on WP 3.8 and up

== Installation ==
1. Upload the plugin files to the `/wp-content/plugins/RealSearchLittle` directory, or install the plugin through the WordPress plugins screen directly.
2. Create a folder called `realsearch` in the `/wp-content/` folder.
3. Allow the web server to read and write files in the `/wp-content/realsearch` folder. (e.g. chmod www-data:www-data realsearch, chmod 777 realsearch )
4. Activate the plugin through the 'Plugins' screen in WordPress
5. Use the 'Admin > RealSearh Little' screen to configure the plugin
6. Press 'Reindex' on the `RealSearch Little` -> `Settings` page

== Frequently Asked Questions ==
= Can it index/search XYZ post type, comments, products? =
Yes. RealSearch can index any post type, even PDFs DOCs etc. 

= The Live Ajax Search looks ugly on my XYZ theme, what can I do =
You can disable the `Live Ajax Search` in the `Settigns` page, or you can add a css file in `/tpl/ajax_search_themes` with the same name as your theme (e.g. xyz.css) and you fix the css issues.

= Keyword highlighting does not work =
This usually means, that the active theme does not use the 'the_excerpt' hook when displaying the search results. You should notify the Theme author, or you can fix it usually by editing the theme's search.php file.

= Can I use it on my Spanish/German/etc website? =
RealSearch will index any content, but will only stem/analyze english, german, and spanish text. If you need support for any other language let me know.


== Screenshots ==
1. Search highlighting matched words.
2. Search statistics.
3. Admin panel settings.
4. Live Ajax serach with highlight.


== Changelog ==
= 1.1.0 =
OpenSource Release
= 1.0.10 =
Initial release
