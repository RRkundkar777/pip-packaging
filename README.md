# Rookie's Guide to deploy a Package

This is a simple example package. You can use
[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
to write your content.

## Extra information for packaging
- [Choosing a license](https://choosealicense.com/)
- [Python packaging user guide](https://packaging.python.org/en/latest/)
- [Overview of python packaging](https://packaging.python.org/en/latest/overview/)
- [Packaging libraries and tools](https://packaging.python.org/en/latest/overview/#packaging-python-libraries-and-tools)
- [Source distribution format](https://packaging.python.org/en/latest/specifications/source-distribution-format/#source-distribution-format)
- [Packaging python projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
- [PyInstaller for Python exe](https://pyinstaller.org/en/stable/)
- [Build backend: Source to distribution package](https://packaging.python.org/en/latest/tutorials/packaging-projects/#choosing-a-build-backend)
- [Version specifier Specification](https://packaging.python.org/en/latest/specifications/version-specifiers/#version-specifiers)
- [Classifiers: Package metadata](https://pypi.org/classifiers/)
- [Project metadata](https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata)
- [Hatch documentation](https://hatch.pypa.io/latest/publish/)
- [Hatch dependency addition](https://hatch.pypa.io/latest/config/dependency/)
- [How a package must look like](https://pypi.org/project/pygame/)


## Commands to build a distribution
- Run build
```shell
python3 -m build
```
- Run publish
```shell
python3 -m twine upload --repository testpypi dist/*
```
- Download your own package
```shell
pip install -i https://test.pypi.org/simple/ example-package-rookie-007==0.0.3
```
- Clean the build
```shell
rm dist/ -r
```