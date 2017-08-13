# Heroku Buildpack for additional build steps

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for web applications that have additional build steps specified in package.json.

## Usage

1. Add script to package.json:

   Set up your build script named `heroku-build` (eg. `webpack -p`)

2. Configure as your second buildpack:

   ```bash
   $ heroku buildpacks:add --index 2 https://github.com/natebot13/heroku-buildpack-webpack
   ```

3. Deploy to Heroku.
