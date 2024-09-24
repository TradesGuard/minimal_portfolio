<script>
    import {
        Collapse,
        NavbarToggler,
        NavbarBrand,
        Nav,
        NavItem,
        NavLink
    } from '@sveltestrap/sveltestrap';

    export let navlist;
    export let personal;

    let isOpen = false;

    function handleUpdate(event) {
        isOpen = event.detail.isOpen;
    }
</script>

<header id="header">
    <div class="header-content">
        <h1>{personal.name}</h1>
       
    </div>
</header>

<style>
    #header {
        padding: 20px 40px;
        background-color: #1C1C1E; /* Dark background for header */
        color: #f8f8f8;
        border-radius: 0 0 10px 10px; /* Rounded bottom edges */
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Subtle shadow for depth */
        width: 100%;
    }

    .header-content {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    h1 {
        font-size: 1.75rem; /* Adjusted font size */
        font-weight: 600;
        margin: 0;
        color: #f8f8f8; /* Ensures the name is visible in a light color */
    }

    .nav-links a {
        color: #f8f8f8;
        text-decoration: none;
        margin-left: 20px;
        font-size: 1rem;
        transition: color 0.3s ease;
    }

    .nav-links a:hover {
        color: #0070f3; /* Accent color on hover */
    }
</style>

