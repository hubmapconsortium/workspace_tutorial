## 05. Create your own template

Templates are pre-set notebooks that can be launched with different datasets. Perhaps you are interested in creating your own template for the Portal.

All templates in the Portal are available in the [user-templates-api repository](https://github.com/hubmapconsortium/user-templates-api).

### Types of templates
There are different ways of creating a template. 

1. The easiest way is to create a Jupyter notebook that uses some simple value insertion to inject e.g. UUIDs. Most templates are created in this way. The instructions for these types of templates are available [here](https://github.com/hubmapconsortium/user-templates-api/blob/development/src/user_templates_api/templates/jupyter_lab/templates/new_template/README.md).

2. There are also other ways of constructing a template. One example is the [Vitessce Visualization template](https://github.com/hubmapconsortium/user-templates-api/blob/development/src/user_templates_api/templates/jupyter_lab/templates/visualization/render.py). This uses a rendering logic to construct the cells of the notebook based on the available data. 

3. There is also the [API tutorial template](https://github.com/hubmapconsortium/user-templates-api/blob/development/src/user_templates_api/templates/jupyter_lab/templates/api_tutorial/render.py), which injects full cells. This way, multiple templates can use the same cells. 

We recommend the first way for most templates, but feel free to chat with us during the office hours about all potential options!

### Helper package
A few functions that help with creating templates, such as a template compatibility checker, are included in a small helper package. Install it as such:

```sh
pip install hubmap-template-helper
```

Read more [here](https://github.com/thomcsmits/hubmap_template_helper).