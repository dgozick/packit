# packit
A fast opinionated front-end build tool that compiles sass/css, vuejs, and js files.

## How-To

###Commands
```bash
packit init
packit watch
packit build
```
### Config
```
{
	"paths": {
		"source": "assets_src",
		"destination": "assets"
	},
	"files": {
		"js": {
			"js/app.js": [
				"/^app\/js\/*"
			]
		},
		"css": {
			"css/app.css": "/app/css/app.css"
		}
	}
}
```

## TODO
* [X] SCSS compiler
* [ ] JS Bundler
  * [ ] [esBuild](https://esbuild.github.io/)
  * [ ] [esBuild Vue Plugin](https://github.com/apeschar/esbuild-vue)
    * Check out [Vitejs.dev](Vitejs.dev) on how it integrates esbuild and Vue
* [ ] Watcher to rebuild files
* [ ] Asset fingerprinting i.e. app.ae3f66.css
