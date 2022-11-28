# Домашнее задание к занятию "`8.3. Gitlab`" - `Мальцев Виктор`

---

### Задание 1

`В качестве ответа добавьте в репозиторий шаблона с решением скриншоты с настройками раннера в проекте.`

![alt text](https://github.com/vmmaltsev/screnshot/blob/main/Screenshot_1.png)
![alt text](https://github.com/vmmaltsev/screnshot/blob/main/Screenshot_2.png)

---

### Задание 2

`В качестве ответа добавьте в шаблон с решением:
- файл gitlab-ci.yml для своего проекта или вставьте код в соответствующее поле в шаблоне,
- скриншоты с успешно собранными сборками.`



```
stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script: 
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .

```

![alt text](https://github.com/vmmaltsev/screnshot/blob/main/Screenshot_3.png)


