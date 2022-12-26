<div>
  <ul>
    <li>l</li>
    <li>i</li>
    <li>g</li>
    <li>h</li>
    <li>t</li>
    <li>i</li>
    <li>n</li>
    <li>g</li>
  </ul>
</div>

<style>
  div {
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 10vh;
    font-family: sans-serif;
    background-color: #272727;
  }

  ul {
    margin: 0;
    padding: 0;
    display: flex;
  }

  ul li {
    list-style: none;
    color: #484848;
    font-size: 80px;
    letter-spacing: 15px;
    animation: lightning 1.4s linear infinite;
    text-transform: uppercase;
  }

  ul li:nth-child(1) {
    animation-delay: 0;
  }
  ul li:nth-child(2) {
    animation-delay: 0.1s;
  }
  ul li:nth-child(3) {
    animation-delay: 0.2s;
  }
  ul li:nth-child(4) {
    animation-delay: 0.3s;
  }
  ul li:nth-child(5) {
    animation-delay: 0.4s;
  }
  ul li:nth-child(6) {
    animation-delay: 0.5s;
  }
  ul li:nth-child(7) {
    animation-delay: 0.6s;
  }
  ul li:nth-child(8) {
    animation-delay: 0.7s;
  }

  @keyframes lightning {
    0% {
      color: #484848;
      text-shadow: none;
    }
    90% {
      color: #484848;
      text-shadow: none;
    }
    100% {
      color: #fff900;
      text-shadow: 0 0 7px #fff900, 0 0 50px #ff6c00;
    }
  }
</style>
