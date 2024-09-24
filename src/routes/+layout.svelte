<script>
    import DATA from '../data/data.js';
    import '../styles/global.css';
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
</script>

<div class="layout">
    <div class="header">
        <Header navlist={DATA.NAVLIST} personal={DATA.PERSONAL} />
    </div>
    <div class="content"> 
        <slot />
    </div>
    <div class="footer">
        <Footer meta={DATA.META} personal={DATA.PERSONAL} contact={DATA.CONTACT} />
    </div>
</div>

<style>
    .layout {
    display: flex;
    flex-direction: column;
    min-height: 100vh; /* Ensure the layout takes the full viewport height */
}

.content {
    flex: 1; /* Allow the content to take up all available space */
}

#header, #footer {
    border-radius: 0 0 10px 10px; /* Rounded bottom edges for the header and top edges for the footer */
}
</style>