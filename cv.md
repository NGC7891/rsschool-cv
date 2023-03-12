# Сергей Сухов

## Frontend разработчик

## Опыт работы


__Think24__ - Работа в большой команде, разработка компонентов на Vue3 c использованием:

- typescript
- provide/inject
- scss
- tailwind
#### Сопровождение кода

- gitlab
- eslint
- настроенный CI/CD
- кодревью

### Мои навыки

- javascript
- typescript
- scss
- сборщик vite (альтернатива webpack)
- vue3
- UI фреймворки
- Figma
- Гибкий и адаптивный как самый лучший web-шаблон 😃
- Коммуникация с коллегами
- Agile методология

### Образование - неоконченное высшее

---

### Пример кода (JavaScript)

```JavaScript
      import { getAngle, getDistance } from "./Calculation.mjs";
      import { checkSphereCollision } from "./Collision.mjs";
      import { conf } from "./SceneConfig.mjs";

      export function updateGravity(frameBuffer) {
        for (let [i, obj1] of frameBuffer.entries()) {
          let acceleration = { accelerationX: 0, accelerationY: 0 };

          // Перебор всех пар объектов и проверка на столкновение друг с другом
          for (let [j, obj2] of frameBuffer.entries()) {
            if (i == j) continue;
            checkSphereCollision(obj1, obj2);
            const distanceObj = getDistance(obj1, obj2);

            const forceMagnitude =
              conf.G *
              ((obj1.mass * obj2.mass) /
                (distanceObj.distance * distanceObj.distance));
            const angle = getAngle(distanceObj.distanceX, distanceObj.distanceY);

            acceleration.accelerationX -= forceMagnitude * Math.cos(angle);
            acceleration.accelerationY -= forceMagnitude * Math.sin(angle);
          }
          obj1.accelerateX = acceleration.accelerationX;
          obj1.accelerateY = acceleration.accelerationY;
        }
      }
```

#### Это модуль с функцией из моего [сайта визитки](https://ngc7891.ru/)



#### Я разработал этот сайт с целью практики следующих технологий:

1. Работа с CANVAS
2. Использование прототипированного наследования (prototype) вместо классов
3. Сборка с помощью Vite
4. Развертывание проекта на VPS(debian)+nginx сервере

#### Планы по улучшению моего сайта:

- Настроить ESLint
- Разобраться и настроить CI/CD, Docker
- Добавить интерактивности
- Поближе познакомиться с архитектурными решениями (паттернами проектирования)

---

### My knowledge of English:
Last year I took private English lessons and worked with a teacher twice a week. Now I can understand the general idea of the videos I watch in English. I can also read texts using Google Translate. I think that my level of English is A2 or B1. I want to continue studying English because I like learning it and I also understand that knowledge of English is absolutely necessary for my career in IT as a frontend developer.


### Мои контакты:
* [GitLab](https://gitlab.com/ngc7891)
* [GitHub](https://gitHub.com/ngc7891)
* [Telegram](https://t.me/NGC7891P)