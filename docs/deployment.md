# Deployment

The project is designed to be self deploying publicly thanks to the `gh-pages` grunt task which is invoked when you run 
```
grunt deploy
```
which will trigger a build, collect all the contents of the `/build` folder, create or clean the `gh-pages` branch of the project, and copy the contents over. This provides an ideal static hosting environment for this project.

# VPS

Since this will likely sit on some server, utilizing a VPS might be a scenario. In that case, this nginx config would work.

```
server {
  listen 80;
  server_name  your.domain.com;

  location / {
    alias /path/to/dir/of/docs;
    index index.html;
  }
}
```