# Svelte_recap

vai in folder nuovo progetto
npx degit sveltejs/template svelte-app
cd svelte-app
npm install

npm i -D autoprefixer node-sass postcss sass svelte-preprocess (per sass)

"pulisci i file prefatti di svelte"

add in file rollup.config.js
	import sveltePreprocess  from 'svelte-preprocess';
	(sotto svelte -> compilerOptions) 
			, 
			preprocess: [
				sveltePreprocess({
					sourceMap: !production,
					postcss: {
						plugins: [require("autoprefixer")],
					},
				}),
			],
		}),
		

(	<style GLOBAL LANG="SCSS">	)   !!!!!!!!!!!!!!!!!

npm run dev (per far partire dev server)
