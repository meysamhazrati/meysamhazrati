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
  technologies: ["HTML", "CSS", "Tailwind", "JS", "React", "Node", "Express", "MongoDB"],
  isCoding: true
}
```

<div align="center">
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"><img src="./icons/html.svg" alt="HTML" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/CSS"><img src="./icons/css.svg" alt="CSS" /></a>
  <a href="https://tailwindcss.com"><img src="./icons/tailwind.svg" alt="Tailwind" /></a>
  <a href="https://javascript.info"><img src="./icons/js.svg" alt="JS" /></a>
  <a href="https://react.dev"><img src="./icons/react.svg" alt="React" /></a>
  <a href="https://nodejs.org"><img src="./icons/node.svg" alt="Node" /></a>
  <a href="https://expressjs.com"><img src="./icons/express.svg" alt="Express" /></a>
  <a href="https://mongodb.com"><img src="./icons/mongodb.svg" alt="MongoDB" /></a>
<div>