<style lang="scss">
    @use '../styles/vars';
    @use 'include-media/dist/include-media' with (
        $breakpoints: vars.$breakpoints
    );

    h1 {
        @include include-media.media('>sm') {
            color: red;
        }

        @include include-media.media('>md') {
            color: blue;
        }
    }

</style>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<!--  -->
