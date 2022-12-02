<svelte:head>
	<title>MateBoy | uses</title>
    <meta http-equiv="Content-Security-Policy" content="default-src 'none'; font-src 'self'; img-src 'self'; script-src 'self' 'unsafe-eval' 'unsafe-inline'; style-src 'self'">
    <meta name="description" content="A page detailing what MateBoy uses as a web developer.">
</svelte:head>

<h1>/uses</h1>
<p>A list of hardware and software I use in my day to day life as a web developer.</p>
<p>More of these pages from other developers can be found <a href="https://uses.tech">here</a>.</p>
<section class="uses-grid">
    <div class="uses">
        <h3>Hardware</h3>
        <ul class="uses-list">
            <li><span>💻</span> MacBook Pro 13", 2020</li>
            <li><span>🖥</span> LG 27UL850-W</li>
            <li><span>⌨️</span> Magic Keyboard</li>
            <li><span>&#128433;&#65039;</span> Logitech MX Master 3</li>
            <li><span>📱</span> iPhone 13 Pro</li>
            <li><span>⌚️</span> Apple Watch Series 4</li>
            <li><span>🎧</span> Sony WH-1000XM4</li>
        </ul>
    </div>
    <div class="uses">
        <h3>Development</h3>
        <ul class="uses-list">
            <li>Main browser: <a href="https://www.mozilla.org/en-US/firefox/developer/">Firefox Developer Edition</a></li>
            <li>Editor: <a href="https://code.visualstudio.com">Visual Studio Code</a></li>
            <li>Theme: <a href="https://github.com/ahmadawais/shades-of-purple-vscode">Shades of Purple</a></li>
            <li>Font: <a href="https://github.com/belluzj/fantasque-sans">Fantasque Sans Mono</a></li>
            <li>Terminal: <a href="https://www.iterm2.com/">iTerm 2</a></li>
        </ul>
    </div>
    <div class="uses">
        <h3>Other software</h3>
        <ul class="uses-list">
            <li>Music: <a href="https://spotify.com">Spotify</a></li>
            <li>Note taking: <a href="https://obsidian.md">Obsidian</a></li>
            <li>Passwords: <a href="https://1password.com">1Password</a></li>
            <li>Learning: <a href="https://apps.ankiweb.net/">Anki</a></li>
            <li>To-do list: <a href="https://culturedcode.com/things/">Things</a></li>
        </ul>
    </div>
</section>

<style>
    h1 {
        margin: 0;
    }

    .uses-grid {
        margin: 5rem 0 0;
    }

    .uses h3 {
        font-size: 1.8rem;
        margin: 0 0 1rem;
    }

    .uses-list {
        padding: 0;
        margin: 0;
        list-style: none;
        font-size: 1.6rem;
    }

    .uses + .uses {
        margin-top: 5rem;
    }

    .uses-list li {
        padding: .5rem 0 .5rem 2rem;
        position: relative;
    }

    .uses-list li > span {
        font-family: system-ui, sans-serif;
    }

    .uses-list li:before {
        content: '';
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: .5rem;
        height: .5rem;
        background-color: #fd7e14;
        border-radius: 50%;
    }

    .theme--dark .uses h3 {
        color: #fd7e14;
    }

    @media screen and (min-width: 768px) {
        .uses-grid {
            display: grid;
            grid-template-columns: auto auto auto;
            grid-gap: 2rem;
            margin: 5rem 0 0;
            width: 100%;
        }

        .uses + .uses {
            margin-top: 0;
        }
    }
</style>