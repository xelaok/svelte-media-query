## svelte-media-query
CSS media queries in svelte.

## Installation

```bash
npm i svelte-media-query
```

## Usage

[Demo](https://svelte.dev/repl/26eb44932920421da01e2e21539494cd)

```html
<script>
    import MediaQuery from "./MediaQuery.svelte";
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
