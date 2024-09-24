<script>
    export let personal;
    export let meta;
</script>

<footer id="footer">
    <div class="footer-content">
        <nav class="footer-links">
            <a href="/">Home</a>
            <a href="/about">About</a>
        
            <a href="/contact">Contact</a>
        </nav>
    </div>
</footer>

<style>
    #footer {
        padding: 20px 0;
        background-color: #1C1C1E; /* Dark background */
        color: #f8f8f8;
        text-align: center;
        border-top: 1px solid #333;
        border-radius: 10px 10px 0 0; /* Soften the footer edges */
        width: 100%;
    }

    .footer-links a {
        color: #f8f8f8;
        text-decoration: none;
        margin: 0 15px;
        transition: color 0.3s ease;
    }

    .footer-links a:hover {
        color: #0070f3; /* Accent color for hover state */
    }
</style>

