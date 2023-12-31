<script>
    import { page } from "$app/stores";
</script>

<h2>About</h2>

<h3>{$page.data.title}</h3>
<div>{@html $page.data.content}</div>