<script>
    import { page } from '$app/stores';
    import { base } from '$app/paths';
</script>

<nav>
    <p>Current URL: {$page.url.pathname}</p>
    <a href="{base}/" class:nav-active-route={$page.url.pathname === `${base}/`}>Home</a>
    <a href="{base}/about" class:nav-active-route={$page.url.pathname === `${base}/about/`}>About</a>
    <a href="{base}/sign-up" class:nav-active-route={$page.url.pathname === `${base}/sign-up/`}>Sign up</a>
</nav>

<style>
    .nav-active-route {
        background-color: hotpink;
    }
</style>