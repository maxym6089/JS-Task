# JS-Task
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <main>
      <div class="element">
        <span class="elementText" id="elementTextId">Text Inside Element</span>
      </div>
      <div class="buttons">
        <button>1: Змінити колір тексту на зелений</button>
        <button>2: Змінити беграунд елемента на синій</button>
        <button>3: Змінити колір рамки на жовтий</button>
        <button>4: Змінити розмір шрифта на 50px</button>
        <button>5: Змінити висоту елемента на 100px</button>
        <button>6: Змінити товщину рамки на 10px</button>
        <button>7: Змінити колір тексту на червоний</button>
        <button>8: Змінити беграунд елемента на жовтий</button>
        <button>9: Змінити колір рамки на синій</button>
        <button>10: Змінити розмір шрифта на 5px</button>
        <button
          onclick="console.log('Click on Element!')"
          onmouseover="console.log('Mouse Over elements')"
          onmouseenter="console.log('Mouse Enter elements')"
          onmouseleave="console.log('Mouse Leave elements')"
        >
          11.a: Змінити висоту елемента на 500px
        </button>
        <button class="changeElementHightTo500">
          11.b: Змінити висоту елемента на 500px
        </button>
        <button class="changeTextToHello">12: Змінити текст на Hello</button>
      </div>
    </main>
  </body>
  <script>
    const changeElementHightTo500El = document.querySelector(
      ".changeElementHightTo500"
    );

    const element22 = document.querySelector(".element");

    changeElementHightTo500El.addEventListener("click", () => {
      element22.style.height = "500px";
    });

    const changeTextToHelloEl = document.querySelector(".changeTextToHello");

    changeTextToHelloEl.addEventListener("click", () => {
      console.log("element22: ", element22);
      /*element22.innerHTML =
        "<span class='elementText' id='elementTextId'>Hello</span>";*/
      /*document.querySelector(".elementText").innerHTML = "Hello!";*/
      element22.querySelector(".elementText").innerHTML = "Hello!!!";
    });

    /*
    const buttonsElement = document.querySelector(".buttons");

    changeElementHightTo500El.addEventListener("click", (event) => {
      console.log("Click 2 on element");
    });

    buttonsElement.addEventListener("click", (event) => {
      console.log("Click on buttons: ", event.target);
      console.log("Click on buttons current: ", event.currentTarget);
    });*/
  </script>
</html>
