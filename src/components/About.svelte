<script>
    let aboutText = "I'm a programer"
    let styles = {darkMode: false}

    function toggle() {
        styles.darkMode = !styles.darkMode;
        window.document.body.classList.toggle('dark-mode');
    }
</script>

<style>
    p {
        color: var(--theme-color);
        font-size: 22px;
    }
</style>

<div class="about">
    <p>{aboutText}</p>
    <button on:click={toggle}>DarkMode {styles.darkMode ? '🌘' : '🌞'}</button>
</div>
