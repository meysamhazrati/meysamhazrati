```javascript
(async () => {
  try {
    const response = await fetch("me");

    if (response.ok) {
      const me = await response.json();
      console.log(me);
    } else {
      const { message } = await response.json();
      throw new Error(message);
    }
  } catch (error) {
    console.error(error);
  }
})();
```

```javascript
{
  firstName: "MeySaM",
  lastName: "HaZraTi",
  birthday: "07-10",
  contact: {
    phone: 09035384705,
    email: "iMeysamHazrati@gmail.com"
  },
  technologies: ["HTML", "CSS"],
  isCoding: true
}
```

<div align="center">
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"><img src="./icons/html.svg" alt="HTML" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/CSS"><img src="./icons/css.svg" alt="CSS" /></a>
<div>