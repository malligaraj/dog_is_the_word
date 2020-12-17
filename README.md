# Dog Breed Identifier

This is a web application that can identify a dog breed from the uploaded image. Currently it can identify 120 different dog breeds. The list of various dog breeds that this website can identify can be found in [Dog Breed Identification dataset description](https://www.kaggle.com/c/dog-breed-identification/data)

This application is based on the Kaggle Competition dataset [Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification). It uses the `fastai` library for training and inference.

This webapp is deployed using [Heroku](https://www.heroku.com/). This webapp is available at https://dog-is-the-word.herokuapp.com/

## Notes
Commands to run the application locally. Run these commands from the root of the repo.
* Build the docker image
```bash
docker build --tag dogistheword:1.0 .
```
* Run the web application from the docker image
```bash
docker run --rm --name mycontainer -p 5000:5000 dogistheword:1.0
```
* Then go to http://localhost:5000/ to view the web page

## Credits:
This project is hugely inspired by the following `Github` repos and took the starter code from these repos.

1. [Pokemon Classifier](https://github.com/sachinchaturvedi93/PokemonClassifier)
2. [fastai starting point to deploy to Render](https://github.com/render-examples/fastai-v3)