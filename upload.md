### Сборка либы
rm -rf dist/ build/ *.egg-info/

python -m build

### Загрузка либы в тест
twine upload --repository testpypi dist/*

### На прод
twine upload dist/*
