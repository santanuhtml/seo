# seo
Gzip Activation:
Gzip compression is an effective way to save bandwidth and speed up your site.
Both W3 Total Cache and WP Super Cache offer Gzip parameters for WordPress and for html add
this code in .htaccess page given below:
-------------------------------
<ifModule mod_gzip.c>
  mod_gzip_on Yes
  mod_gzip_dechunk Yes
  mod_gzip_item_include file \.(html?|txt|css|js|php|pl)$
  mod_gzip_item_include handler ^cgi-script$
  mod_gzip_item_include mime ^text/.*
  mod_gzip_item_include mime ^application/x-javascript.*
  mod_gzip_item_exclude mime ^image/.*
  mod_gzip_item_exclude rspheader ^Content-Encoding:.*gzip.*
</ifModule>
-------------------------------
url: https://www.ostraining.com/blog/webdesign/use-gzip-to-speed-up-your-cms-powered-website/
