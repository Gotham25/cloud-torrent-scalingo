
# Installation for Scalingo

To deploy cloud-torrent on Scalingo, just click on this button:

[![Deploy on Scalingo](https://cdn.scalingo.com/deploy/button.svg)](https://dashboard.scalingo.com/create/app?source=https://github.com/Gotham25/cloud-torrent-scalingo#main)

or using CLI:

```
git clone https://github.com/Gotham25/cloud-torrent-scalingo.git cloud-torrent && cd cloud-torrent
scalingo create cloud-torrent
scalingo --app cloud-torrent env-set AUTHENTICATED=no
scalingo --app cloud-torrent env-set AUTH_USERNAME=admin
scalingo --app cloud-torrent env-set AUTH_PASSWORD=admin
scalingo --app cloud-torrent env-set BUILDPACK_URL=https://github.com/Scalingo/php-buildpack
git push scalingo main
```
