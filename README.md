# twitter-no-promoted-tweets-javascript snippet
So, promoted tweets are pretty annoying. Good thing as developers, we know how to handle that.

---

> **_If you're a dev, you'll know how to use this. Use this at your own risk._**

---

I've tested this on chrome. In theory it should work on all others, but I haven't actually tested that. "It works for me", is a sataisfactory answer for me. I offer No warranty.**You're on your own pal**.

---

# Behold, The Code!

```javascript
addEventListener("scroll", (event) => { 
    [...document.querySelectorAll("span")].filter(el => el.innerText === "Promoted" ? el.parentElement.parentElement.parentElement.parentElement.parentElement.parentElement.parentElement.remove():null)
    }
);

```

