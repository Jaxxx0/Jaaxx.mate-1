
# my site4

I write about technology.
http://feelcame.github.io/




## Running a local server
```
bundle install
jekyll serve
```


If it throws errors, dependencies may not be installed
```
bundle install
```


## TO DO

- “Up” button to fly to the bottom right
- ability to change the appearance of the list of articles: in a line or in blocks
- a design similar to that of Spotify was recently made in the form of cards. Vastrick has the same cards
- add shadow to pictures. here is an example <http://shpargalkablog.ru/2013/06/youtube.html>
- Create an admin userscript. So that it is stored in local storage. And it was executed on each page where a master script was connected that would load the main one and execute it. You need to make a custom admin panel for a static site
- Make the search not a page, but a pop-up field under the header. Pressing enter or clicking on the search button opens a new page with the same input field and offline search for Jason. And also three radio buttons: by site, by repo, via Google
- make the buttons in the mobile menu not only open but also close the search/navigator

- comments. design buttons. arrange in a line on computers and in a column on phones
- add another comment button: “in telegram tg://”, “in a new tab” and “right here”

- when searching, expand all spoilers
- also rewrite the highlighting script so that all occurrences on the page are highlighted

- Make something like a PWA from the site (you need to register manifest.json). Load the entire site into the cache (\_pages folder). Check for updates using Javascript. And write the date below

- make lists in blocks in two columns
  ```
    style: 'ul{overflow:hidden;flex-wrap:wrap} ul{/*display:table;flex-wrap:wrap*/;display:flex;flex-flow:row wrap;padding:0} ul li{text-align:center;float:left;box-sizing:border-box;width:calc(50% - 8px);padding:7px 10px;background:#eee;margin:4px;list-style-type:none;min-height:50px;/*height:5em;*/padding-left:15px;padding-right:15px;border-radius:10px}'
  ```

- custom feedback form


## List of changes
- Collapsible navigation for phones
- Make comments activated via parameter
- when you press open navigation on your phone, you don’t need to follow the link.
- sort in dir-ls.md by the index field. and if its value < 0, then hide the page from the output
- So that pressing the up button expands the navigation and notifies about this with a line above “content”
- Add three navigation buttons to the site in the mobile version instead of one. Home, search, sandwich to open a list of categories. They will have to be duplicated for the phone and for the PC; it will not be possible to distribute them through styles. Through a media query, find out that the site is open on the phone and hide the home and search buttons on the computer.
- When you click on the sandwich, category buttons should appear above the Three buttons. Accordingly, you get a cake of categories and three pillars on which it lies

## useful links

- [Spoiler customization](http://shpargalkablog.ru/2013/04/details-html.html)
