<div>
  <a href="#"> button hover effect</a>
</div>

<style>
  div {
    height: 10vh;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: verdana;
  }

  a {
    width: 300px;
    height: 60px;
    text-decoration: none;
    text-transform: uppercase;
    background-color: transparent;
    text-align: center;
    line-height: 60px;
    font-weight: bold;
    letter-spacing: 2px;
    position: relative;
    transition: all 0.2s;
    color: white;
  }

  a:before {
    content: "";
    position: absolute;
    top: -3px;
    left: -3px;
    width: 100%;
    height: 100%;
    background-color: #20caff;
    z-index: -1;
    mix-blend-mode: multiply;
    transition: all 0.2s;
    transform-origin: top;
  }

  a:after {
    content: "";
    position: absolute;
    top: 3px;
    left: 3px;
    width: 100%;
    height: 100%;
    background-color: #ff7675;
    z-index: -1;
    mix-blend-mode: multiply;
    transition: all 0.2s;
    transform-origin: bottom;
  }

  a:hover:before {
    top: -6px;
    left: 0;
    transform: perspective(1000px) rotateX(75deg);
  }

  a:hover:after {
    top: 6px;
    left: 0;
    transform: perspective(1000px) rotateX(-75deg);
  }

  a:hover {
    color: #272727;
  }
</style>
