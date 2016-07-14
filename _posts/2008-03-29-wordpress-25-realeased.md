---
id: 73
title: WordPress 2.5 realeased!
date: 2008-03-29T15:28:51+00:00
author: Kit
layout: post
guid: http://rivalrockets.com/blog/?p=73
permalink: /2008/03/wordpress-25-realeased/
dsq_thread_id:
  - 77580417
categories:
  - Blog
---
### I copped this right off of the WordPress.org page:

<!--more-->

> ### User Features
> 
> **Cleaner, faster, less cluttered dashboard** â€” weâ€™ve worked hard to take your feedback about whatâ€™s most important in the dashboard and organize things to allow you to focus on whatâ€™s important â€” your blog â€” and get out of your way. In collaboration with [Happy Cog](http://happycog.com/) and the community weâ€™ve taken the first major step forward in the WordPress interface since version 1.5.
> 
> **Dashboard Widgets** â€” the dashboard home page is now a serious of widgets, including ones to show you fun stats about your posting, latest comments, people linking to you, new and popular plugins, and of course WordPress news. You can customize any of the dashboard widgets to show, for example, news from your local paper instead of WP news. Plugins can also hook in, for example the [WordPress.com stats widget](http://wordpress.org/extend/plugins/stats/) adds a handy double-wide stats box.
> 
> **Multi-file upload with progress bar** â€” before when you would upload a large file youâ€™d wait forever, never knowing how far along it was. And uploading more than one photo was an exercise in patience, as you could only do one at a time. Now you can select a whole of folder images or music or videos at once and itâ€™ll show you the progress of each upload.
> 
> **Bonus: EXIF extraction** â€” if you upload JPEG files with EXIF metadata like camera make and model, aperture, shutter speed, ISO, et al. WordPress will extract all the data into custom fields you can use in your template. If you use the EXIF title fields or similar those will be put into their equivalent fields in WP. Most modern digital cameras generate EXIF data.
> 
> **Search posts and pages** â€” search used to cover just posts, now it includes pages too, a great boon for thoe using WordPress as a CMS. New themes can style or sort pages differently in results.
> 
> **Tag management** â€” you can now add, rename, delete, and do whatever else you like to tags from inside WordPress, no plugins needed.
> 
> **Password strength meter** â€” when you change your password on your profile itâ€™ll tell you how strong your password is to help you pick a good one.
> 
> **Concurrent editing protection** â€” for those of you on multi-author blogs, have you ever opened a post while someone was already editing it, and your auto-saves kept overwriting each other, irrecoverably losing hours of work? I bet that added a few words to your vocabulary. Now if you open a post that someone else is editing, WordPress magically locks it and prevents you from saving until the other person is done. Youâ€™ll see a message like below.
> 
> **Few-click plugin upgrades** â€” if the plugins you use are part of the plugin directory since 2.3 weâ€™ve told you when they have an update available. Now we take that to the next logical step â€” downloading and installing the upgrade for you. This is dependent a little bit on your host setup, and it may ask you for your FTP password much like OS X or Windows will ask you for a password, but it works well on majority of hosts we were able to test, your mileage may very, plugins in mirror may be larger than they appear.
> 
> **Friendlier visual post editor** â€” Iâ€™m not sure how to articulate this improvement except to say â€œit doesnâ€™t mess with your code anymore.â€ Weâ€™re now using version 3.0 of TinyMCE, which means better compatibility with Safari, and weâ€™ve paid particular attention this release to its integration and interaction with complex HTML. It also now has a â€œno-distractionsâ€ mode which is like Writeroom for your browser.
> 
> **Built-in galleries** â€” when you take advantage of multi-file upload to upload a bunch of photos, we have a new shortcode that lets you to easily embed galleries by just putting \[ gallery\] (without the space) in your post. Itâ€™ll display all your thumbnails and captions and each will link each to a page where people can comment on the individual photos. Iâ€™ve been using this feature on my blog and have already uploaded over [1,200 pictures into 23 galleries](http://ma.tt/category/gallery/). The shortcode has some hidden options too, [check out this documentation](http://codex.wordpress.org/Using_the_gallery_shortcode).
> 
> ### Developer Features
> 
> Now for the geeky stuff. While weâ€™re excited about the above features, each one represents a new opportunity or API for other developers to take to another level. (The best of which weâ€™ll someday integrate back into WP.)
> 
> **Salted passwords** â€” we now use the [phpass](http://www.openwall.com/phpass/) library to stretch and salt all passwords stored in the database, which makes brute-forcing them impractical. If you use something like [mod\_auth\_mysql](http://modauthmysql.sourceforge.net/) weâ€™ve [created a plugin that will allow you to use legacy MD5 hashing](http://wordpress.org/extend/plugins/md5-password-hashes/). (The hashing is completely pluggable.) Users will automatically switch to the more secure passwords next time they log in.
> 
> **Secure cookies** â€” cookies are now encrypted based on the protocol described [in this PDF paper](http://www.cse.msu.edu/%7Ealexliu/publications/Cookie/cookie.pdf). which is something like `user name|expiration time|HMAC( user name|expiration time, k)` where `k = HMAC(user name|expiration time, sk)` and where `sk` is a secret key, which you can define in your config.
> 
> **Easy taxonomy and URL creation** â€” probably best illustrated with an example: I can call `register_taxonomy()` with [a few arguments](http://trac.wordpress.org/attachment/ticket/6357/taxes.php) to register a â€œpeopleâ€ taxonomy and whenever I edit an image Iâ€™ll see a UI like tags has for identifying the people in a photo, and these will be URL addressable with `/person/firstname-lastname/`. All with a single function call.
> 
> **Inline documentation** â€” the vast majority of the new code going into WordPress include inline documentation that explains the functions and documents their arguments.
> 
> **Database optimization** â€” we havenâ€™t changed the table layout in this release, which is one of the reasons so many plugins work fine with 2.5. We have added a few new indicies and made a few default fields more flexible based on some bottlenecks we found on WordPress.com, which now hosts 2.7 million WordPress blogs. It should be invisible to the application, just a bit faster on the database side.
> 
> **$wpdb->prepare()** â€” now almost all of the SQL in WordPress is prepared first, and the same functions are available to your plugins. This should prevent elementary SQL escaping issues.
> 
> **Media buttons** â€” the add media buttons above the post are both expandable, so you could have an â€œAdd Google Mapâ€ button if you like, They can be overridden, so if you think you can do the video or audio tab better than we have you can replace the default.
> 
> **Shortcode API** â€” the new gallery functionality is powered by the new shortcode API. Shortcodes are little bracket-delineated strings that can be magically expanded at runtime to something more interesting. They give users a short, easy to type and copy/paste string they can move around their post without worrying about messing up complex HTML or embed codes. [The Shortcode API is fully documented](http://codex.wordpress.org/Shortcode_API).