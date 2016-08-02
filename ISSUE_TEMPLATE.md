### URL

http://my.customurl.com/service

### LOGO

http://my.customurl.com/service/logo.png

### Unread Code

```javascript
function checkUnread() {
    var e = document.getElementsByClassName("unread_countValue");
    var t = 0;
    for( i = 0; i < e.length; i++ ) t += parseInt(e[i].innerHTML.trim());
    updateBadge(t);
}

function updateBadge(e) {
    e >= 1 ? document.title = "(" + e + ") " + originalTitle : document.title = originalTitle
}
var originalTitle = document.title;
setInterval(checkUnread, 3000);
```
