git remote add - Привязать удалённый репозиторий к локальному

Перейдите на страницу удалённого репозитория: https://github.com/USER_NAME/REPOSITORY_NAME, выберите тип `SSH` и скопируйте URL.

Откройте консоль, перейдите в каталог локального репозитория и введите команду `git remote add` (от англ. _remote_ — «удалённый» и _add_ — «добавить»).

```bash
git remote add origin git@github.com:USER_NAME/REPOSITORY_NAME.git 
```

Команде необходимо передать два параметра: имя удалённого репозитория и его URL. В качестве имени используйте слово `origin`. А URL вы скопировали со страницы удалённого репозитория.
`origin` (англ. «источник») — стандартный псевдоним, с помощью которого можно обращаться к главному удалённому репозиторию (обычно такой репозиторий один). Это значительно упрощает работу.

## Убедиться, что репозитории связаны, — `git remote -v`
```bash
git remote -v
```

Флаг `-v` — короткая форма флага `--verbose` (англ. «подробный»). Он позволяет показать больше информации в выводе.
```bash
git remote -v
origin    git@github.com:%ИМЯ_АККАУНТА%/%ИМЯ_ПРОЕКТА%.git (fetch)
origin    git@github.com:%ИМЯ_АККАУНТА%/%ИМЯ_ПРОЕКТА%.git (push) 
```

В выводе должны быть строчки, аналогичные тем, что показаны выше.