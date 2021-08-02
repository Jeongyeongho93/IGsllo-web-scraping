# IGsllo-web-scraping

/* Could use this, might be slower/less robust */
* filename src url "https://www.instagram.com/explore/tags/sllo/";

/*prefer PROC HTTP for speed and flexibility*/
filename src temp;
proc http
 method="GET"
 url="https://www.instagram.com/explore/tags/sllo/"
 out=src;
run;
