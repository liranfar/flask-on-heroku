# flask-on-heroku
Heroku is a PaaS which allows you to deploy your app automatically on their containers called "dyno". All the container instructions should be found in `Procfile`.

## Usage

1. Clone this repo
1. Create a user in Heroku
1. Install herokuCLI: `$ curl https://cli-assets.heroku.com/install-ubuntu.sh | sh`
1. Create a new heroku app :
```
$ heroku login
$ heroku create <your-app-name>
```
1. Run the following command for deployment:
``` bash
cd flask-on-heroku
$ heroku git:remote flask-deploy-blog-liran
$ git push heroku master
```

## TODO
1. Add postgreSQL persistency.

## Resources
* [Matt Huddleston blog post](https://progblog.io/How-to-deploy-a-Flask-App-to-Heroku/)

* [The Flask Mega Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xviii-deployment-on-heroku)

* [Heroku Official Site](https://dashboard.heroku.com/)
* [John Kagga blog post](https://medium.com/the-andela-way/deploying-a-python-flask-app-to-heroku-41250bda27d0)

* [Why we don't use nginx in heroku ?](https://stackoverflow.com/questions/33286651/on-heroku-is-it-safe-to-run-gunicorn-out-in-front)

## Extra
* [The advantages of using nginx as a reverse-proxy server in IaaS. (a hint: buffering)](https://serverfault.com/questions/220046/why-is-setting-nginx-as-a-reverse-proxy-a-good-idea)
