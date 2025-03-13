# WorldGuessr - Locate
This script locates your position and opens the location on Google Maps in a new tab.

*You can save the script as a bookmark, or paste into inspect element's console.*

```js
javascript:(()=>{if (!document.querySelector(".svframe")) return alert("You must be in a WorldGuessr game for this to work!");const q = new URLSearchParams(`?${document.querySelector(".svframe").src.split("?")[1]}`);window.open(`https://google.com/maps/search/${q.get("lat")},${q.get("long")}`);})()
```
