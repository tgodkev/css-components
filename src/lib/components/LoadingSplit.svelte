<div>
  <div class="loader">
    <span class="top-half">loading</span>
    <span class="bottom-half">loading</span>
  </div>
</div>

<style>
  div {
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 10vh;
    font-family: sans-serif;
  }

  .loader {
    width: 300px;
    height: 60px;
    border: 7px solid #0a3d62;
    border-radius: 10px;
    text-align: center;
    line-height: 60px;
    position: relative;
    overflow: hidden;
  }

  span {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    font-size: 48px;
    text-transform: uppercase;
    font-weight: 600;
  }

  .top-half {
    color: #ee5253;
    clip-path: polygon(0 0, 100% 0, 100% 50%, 0 50%);
    animation: split 4s linear infinite;
  }

  .bottom-half {
    color: #0a3d62;
    clip-path: polygon(0 50%, 100% 50%, 100% 100%, 0 100%);
    animation: split 4s linear infinite reverse;
  }

  @keyframes split {
    0% {
      transform: translateX(100%);
    }
    40% {
      transform: translateX(0);
    }
    60% {
      transform: translateX(0);
    }
    100% {
      transform: translateX(-100%);
    }
  }
</style>
