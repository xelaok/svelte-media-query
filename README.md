## svelte-media-query ([npm](https://www.npmjs.com/package/svelte-media-query), [demo](https://svelte.dev/repl/26eb44932920421da01e2e21539494cd))
CSS media queries in svelte.

## Installation

```bash
npm i svelte-media-query
```

## Usage

```html
<script>
    import MediaQuery from "svelte-media-query";
</script>

<MediaQuery query="(min-width: 1281px)" let:matches>
    {#if matches}
    <div class="root default">
        default
    </div>
    {/if}
</MediaQuery>

<MediaQuery query="(min-width: 481px) and (max-width: 1280px)" let:matches>
    {#if matches}
    <div class="root tablet">
        tablet
    </div>
    {/if}
</MediaQuery>

<MediaQuery query="(max-width: 480px)" let:matches>
    {#if matches}
    <div class="root mobile">
        mobile
    </div>
    {/if}
</MediaQuery>
```
