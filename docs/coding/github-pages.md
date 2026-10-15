# Using Material for MkDocs with GitHub Pages

This page includes step-by-step instructions as well as helpful tips for utilizing Material for MkDocs to serve your GitHub documentation (it is what this site is running on right now).

## Getting Started

### GitHub Pages

To get your GitHub Pages site up and running, follow the steps [documented by GitHub](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site#creating-your-site).

The best Material for MkDocs resource currently available is hosted at [squidfunk.github.io](https://squidfunk.github.io/mkdocs-material/reference). There are a ton of examples on different styling and extensions to use with mkdocs.

### Spinning up Locally

For spinning up locally, you'll be using a Virtual Environment (venv). You'll need to have Python 3.7 or later installed as well as Visual Studio Code.

#### Initial Setup

1. Clone your repository.
2. From your repository root, create and activate your venv using the following commands.
  ``` code
    python -m venv .\venv
    .\venv\Scripts\activate.bat
  ```

    !!! note
        if Python is not found, you may need to add it to your PATH

3. Next you'll install requirements using the following command.
  ``` code
    pip install -r requirements.txt
  ```

    !!! note 
        Here is a list of the dependencies used in this repository. (1)
        { .annotate }

        1.  attrs<br>
            beautifulsoup4<br>
            bleach<br>
            certifi<br>
            cffi<br>
            charset-normalizer<br>
            click<br>
            colorama<br>
            cryptography<br>
            defusedxml<br>
            entrypoints<br>
            fastjsonschema<br>
            ghp-import<br>
            gitdb<br>
            GitPython<br>
            idna<br>
            importlib-metadata<br>
            Jinja2<br>
            jsonschema<br>
            jupyter-client<br>
            jupyter-core<br>
            jupyterlab-pygments<br>
            Markdown<br>
            MarkupSafe<br>
            mergedeep<br>
            mistune<br>
            mkdocs<br>
            mkdocs-autolinks-plugin<br>
            mkdocs-awesome-pages-plugin<br>
            mkdocs-glightbox<br>
            mkdocs-material<br>
            mkdocs-material-extensions<br>
            mkdocs-monorepo-plugin<br>
            mkdocs-open-in-new-tab<br>
            mknotebooks<br>
            nbclient<br>
            nbconvert<br>
            nbformat<br>
            nest-asyncio<br>
            packaging<br>
            pandocfilters<br>
            pycparser<br>
            pygments<br>
            PyJWT<br>
            pymdown-extensions<br>
            pyparsing<br>
            pyrsistent<br>
            python-dateutil<br>
            python-slugify<br>
            pywin32; sys_platform == "win32"<br>
            PyYAML<br>
            pyyaml-env-tag<br>
            pyzmq<br>
            requests<br>
            six<br>
            smmap<br>
            soupsieve<br>
            text-unidecode<br>
            tinycss2<br>
            tornado<br>
            traitlets<br>
            urllib3<br>
            watchdog<br>
            webencodings<br>
            zipp

4. Serve locally using the following command.
  ``` code
    mkdocs serve
  ```

    !!! note
        Mkdocs serve will serve your site at: http://127.0.0.1:8000/ and will listen for changes as you develop in your IDE.

#### Going Forward

After you've run the intial setup steps above (cloning your repo, creating your venv, installing requirements) it's fairly simple to serve your project locally. You'll just need to follow these steps:

1. Navigate to your repo directory
2. Activate your venv (.\venv\Scripts\activate.bat)
3. Serve! (mkdocs serve)
