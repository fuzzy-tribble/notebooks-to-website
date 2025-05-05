# Template for Displaying NBs Repos

Tmeplate/example for displaying a repository with Jupyter Notebooks as a static website using github pages

## Usage

- Put all notebooks in the `notebooks` folder
- Configure website however you want in the `website/_config.yml` file
- Enable github pages in the repository settings

Commit and push changes and the github action workflow will build the website on a new branch `gh-pages` and deploy it to the `gh-pages` branch. It builds the ipynb files to html using `nbconvert` and putting them in the `website/_notebooks` folder. The `website` folder is the root of the github pages site. The `gh-pages` branch is the branch that github pages uses to serve the website.

You can then view the website at `https://<username>.github.io/<repo-name>/` or `https://<username>.github.io/` if you have a custom domain.