<script lang="ts">
  const seed: string = "";
  const animate = (): void => {
    console.warn("animate");
  };
</script>

<div id="blob">Hello world</div>

<style>
  #blob {
    width: 200px;
    height: 200px;
    border-radius: 50% 50% 50% 50% / 30% 30% 30% 30%;
    background-color: pink;
    animation: stand 2s infinite;
    animation-timing-function: ease-in-out;
    animation-direction: alternate-reverse;
  }

  @keyframes stand {
    from {
      width: 200px;
      height: 200px;
    }
    to {
      width: 300px;
      height: 100px;
      border-radius: 30% 45% 67% 12% / 57% 89% 34% 22%;
    }
  }
</style>
