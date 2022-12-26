<div>
  <h1>css animation</h1>
</div>

<style>
  div {
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 10vh;
    font-family: sans-serif;
    background-color: #273c75;
  }

  h1 {
    font-size: 60px;
    text-align: center;
    text-transform: uppercase;
    background: url(image.jpg);
    background-clip: text;
    color: transparent;
    animation: textBackground 10s linear infinite;
  }

  @keyframes textBackground {
    0% {
      background-position: 0 0;
    }
    100% {
      background-position: 100% 100%;
    }
  }
</style>
