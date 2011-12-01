## manifestR: get your sites offline

HTML5 features appcaching, a way to make your web sites and apps work
offline, and to increase their performance as well.

To learn more about the HTML5 appcache, [read our comprehesive
overview][] to get you started.

### So what does manifestR do?

manifestR is a bookmarklet, which you drag to your bookmarks bar. Then,
when you visit any page, you can click the manifestR button, and it will
create an HTML5 appcache manifest file for that page. For more on how
you then use the manifest [see our article][].

### How do I use it?

-   Step 1: drag [manifestR][] (that’s the link just to the left of
    this) to the bookmarks bar in your browser
-   Step 2: visit any web page you want to create an HTML5 appcache
    manifest for
-   Step 3: click the manifestR button in your bookmarks bar
-   Step 4: copy the manifest it creates
-   Step 5: [read on][see our article] for how to work with appcache to
    take your web sites and apps offline

### What does manifestR do?

When you use ManifestR on a page, here’s what it looks for

-   images both in the same and other domains referenced in the src
    attribute of any img element in the page.
-   links to pages in the same domain. This can improve the performance
    of your site for visitors viewing other pages, and is vital if you
    want the entire site/​app to work offline, but means potentially
    considerable additional load on your server the first time someone
    visits the site. Whether you choose to keep this list, or remove
    some or all of the links is an important decision to make.
-   style sheets, linked, or included via @import statements, located
    both in your domain, or other domains
-   images linked to in any style sheet, both those in the same domain,
    or other domains
-   JavaScript files, both those in the same domain, and served from
    other domains. Here too, you’ll need to consider carefully which to
    include and which you want to add to the online whitelist via the
    NETWORK section of the manifest.
-   it then puts them all together in a manifest, ready for you to cut
    and paste, tweak, save and upload.

### What’s next?

-   Follow me on [twitter][] to keep up to date with manifestR
    developments
-   explore the other [tools][] we have here to help you better work
    with HTML5 and CSS3
-   Take a look at the [conferences we run][] for web developers like
    you, including [Web Directions South][] in Sydney in October each
    year.

  [read our comprehesive overview]: http://www.webdirections.org/blog/get-offline/
  [see our article]: http://www.webdirections.org/blog/get-offline
  [manifestR]: javascript:function%20loadScript(scriptURL)%20%7B%20var%20scriptElem%20=%20document.createElement('SCRIPT');%20scriptElem.setAttribute('language',%20'JavaScript');%20scriptElem.setAttribute('src',%20scriptURL);%20document.body.appendChild(scriptElem);%7DloadScript('http://westciv.com/tools/manifestR/manifestR.js');
  [twitter]: http://twitter.com/johnallsopp
  [tools]: http://westciv.com/tools/index.html
  [conferences we run]: http://webdirections.org
  [Web Directions South]: http://south11.webdirections.org/
