<script lang="ts">
  import { LightSwitch } from "@skeletonlabs/skeleton";
  import { page } from "$app/stores";

  const title = "MatEs";
  const description =
    "Donde la lógica y la creatividad se encuentran. ¡Únete a nuestros talleres y grupos de estudio!";
  const url = `https://${$page.url.host}`;
</script>

<svelte:head>
  <title>{title}</title>
  <meta name="description" content={description} />

  <meta property="og:type" content="website" />
  <meta property="og:url" content={url} />
  <meta property="og:title" content={title} />
  <!-- <meta property="og:image" content="https://example.com/image.jpg" /> -->
  <meta property="og:description" content={description} />
  <meta property="og:locale" content="es_EC" />
  <meta name="twitter:card" content="summary" />
  <meta name="twitter:url" content={url} />
</svelte:head>

<div class="container mx-auto grid h-full place-items-center">
  <div class="space-y-5">
    <h1 class="h1">{title}</h1>
    <p>Start by exploring:</p>
    <ul>
      <li>
        <code class="code">/src/routes/+layout.svelte</code> - barebones layout, the CSS import order
        is critical!
      </li>
      <li>
        <code class="code">/src/app.postcss</code> - minimal css to make the page full screen, may not
        be relevant for your project
      </li>
      <li>
        <code class="code">/src/routes/+page.svelte</code> - this page, you can replace the contents
      </li>
    </ul>
    <div class="grid place-items-center">
      <LightSwitch />
    </div>
  </div>
</div>
