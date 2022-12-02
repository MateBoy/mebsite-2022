<div class="main-wrap">
    <header class="header">
        <nav class="nav">
            <a href="/" class="nav__link home">Home</a>
            <a href="/uses" class="nav__link">Uses</a>
            <!-- <a class="nav__link" title="Digital Garden" href="https://mateboy.gitbook.io/knowledge-base/">🌱</a> -->
        </nav>
    </header>
    <main class="main">
        <slot/>
    </main>
    <footer class="footer">
        <p>Made with <a href="https://kit.svelte.dev/">SvelteKit</a> and <a href="https://netlify.com">Netlify</a>.</p>
    </footer>
</div>

<style>
.main-wrap {
    width: 100%;
}

.main {
	flex-grow: 1;
	padding: 0 2rem;
}

.nav {
	padding: 0 2rem;
}

.header {
	padding: 2.4rem 0;
	margin-bottom: 2.4rem;
	border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.nav__link {
	text-decoration: none;
	color: #868e96;
	font-size: 1.5rem;
}

.nav > * + * {
	margin-left: 3rem;
}

.nav .nav__link {
	color: #adb5bd;
}

.footer {
	margin-top: 3rem;
	padding: 1rem 2rem;
	border-top: 1px solid rgba(255, 255, 255, 0.1);
}

.footer p {
	font-size: 0.8em;
}

@media screen and (min-width: 768px) {
	.main {
		max-width: 800px;
		margin: 0 auto;
		padding: 0 20px;
	}

	.header {
		margin-bottom: 4rem;
		padding: 2rem 0;
	}

	.nav {
		display: block;
		max-width: 800px;
		margin: 0 auto;
		padding: 0 20px;
	}

	@supports (display: flex) {
		.main-wrap {
			display: flex;
			flex-direction: column;
			min-height: 100vh;
		}
	}

	.footer {
		color: #868e96;
		padding: 1.4rem 20px;
		margin: 6rem auto 0;
		width: 100%;
		text-align: center;
	}
}

@media screen and (min-width: 1024px) {
	.main {
		width: 800px;
	}

	.nav {
		width: 800px;
	}
}
</style>