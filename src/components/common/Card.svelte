<style>
  img {
    animation-duration: 1s;
    animation-fill-mode: both;
    animation-name: fadeIn;
    box-shadow: 0 10px 60px 0 rgb(0 0 0 / 20%);
    border-radius: 5px;
    max-width: 400px;
  }

  img.large {
    max-width: 600px;
  }

  @media (max-width: 900px) {
    img {
      max-width: 100%;
    }
    img.large {
      max-width: 100%;
    }
  }
</style>

<script lang="ts">
  export let title: string
  export let size: string = 'normal'
  export let backgroundUrl: string
  export let readMoreUrl: string = undefined
</script>

<div>
  <img class="{size}" src="{backgroundUrl}" alt="{`${title}-drop`}" />
  <h3>{title}</h3>
</div>
