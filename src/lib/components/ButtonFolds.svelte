<div>
  <a href="#">Button</a>
</div>

<style>
  div {
    height: 20vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #212121;
    font-family: sans-serif;
  }

  a {
    padding: 20px 40px;
    text-decoration: none;
    text-transform: uppercase;
    background-color: #f1c40f;
    color: white;
    font-size: 20px;
    letter-spacing: 2px;
    position: relative;
  }

  a:before {
    content: "Button";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #2ce771;
    display: flex;
    justify-content: center;
    align-items: center;
    transform: rotateX(270deg);
    transform-origin: top;
    transition: all 0.5s;
  }
  a:after {
    content: "Button";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: red;
    display: flex;
    justify-content: center;
    align-items: center;
    transform: rotateX(270deg);
    transform-origin: bottom;
    transition: all 0.5s;
    transition-delay: 0.25s;
  }

  a:hover:before {
    transform: rotateX(0);
  }
  a:hover:after {
    transform: rotateX(0);
  }
</style>
