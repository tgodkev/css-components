<script lang="ts">
</script>

<div>
  <a href="#">Hover Me</a>
</div>

<style>
  div {
    height: 20vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  a {
    padding: 40px 80px;
    font-family: sans-serif;
    text-decoration: none;
    color: #262626;
    font-size: 45px;
    letter-spacing: 2px;
    border: 5px solid #262626;
    position: relative;
    transform: 1s;
  }

  a:before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 101%;
    height: 100%;
    background-color: #262626;
    transition: 1s;
    transform: rotateX(90deg);
    z-index: -1;
  }

  a:after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 101%;
    height: 100%;
    background-color: #262626;
    transition: 1s;
    transform: rotateY(90deg);
    z-index: -1;
  }

  a:hover:before,
  a:active:before {
    transform: rotateX(0);
  }
  a:hover:after,
  a:active:after {
    transform: rotateY(0);
  }

  a:hover,
  a:active {
    color: white;
  }
</style>
