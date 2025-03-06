# 🤖 BoredBot

Welcome to **BoredBot**!  
This is a simple and fun project I built while learning from the **[Scrimba Frontend Developer Career Path](https://scrimba.com/)**. The BoredBot helps you find random activities when you're feeling bored by fetching suggestions from an API.

---

## 🌟 What is BoredBot?

BoredBot is a small web app that uses the [Bored API](https://www.boredapi.com/) to suggest random activities. Every time you click the button, BoredBot fetches a new activity idea to help cure your boredom.

---

## 🚀 JavaScript Explanation (`index.js`)

The core logic of BoredBot revolves around the **`fetch()`** method, which allows us to make network requests to get data from APIs.

Here's the code:

```javascript
document.getElementById("get-activity").addEventListener("click", function() {
  fetch("https://apis.scrimba.com/bored/api/activity")
    .then(response => response.json())
    .then(data => {
      document.getElementById("activity").textContent = data.activity
      document.getElementById("title").textContent = "🦾 HappyBot🦿"
      document.querySelector("main").classList.add("fun")
    })
})
```

## 📚 What I learned
- Working with APIs using fetch()
- Handling asynchronous data
- DOM manipulation
- Adding dynamic interactivity to web pages
- Writing accessible HTML (with ARIA attributes)
## 🙏 Acknowledgments
Special thanks to Scrimba for the tutorial that guided me through building this project. Their interactive and hands-on approach makes learning frontend development really fun!

## 📌 Future improvements
- Add loading indicators while fetching data.
- Show different categories of activities.
- Improve the button design with better hover effects.
- Add offline fallback content.
