# Настройка VS Code для разработки. Конфигурирование дебагера для Node.js

1. Зайдите в раздел с расширениями.
2. Установите плагины GitLens, Prettier, Eslint, Beautify.
3. Сконфигурируйте Eslint. Варианты правил, чтобы код проверялся при сохранении, есть по ссылке. Инструкция доступна по ссылке.
4. Сконфигурируйте Prettier, чтобы при сохранении форматировался код.
5. Создайте конфигурацию дебагера для отладки js с использованием Node.js.
6. Чтобы проверить, что конфигурация под Node.js работает, нужно:

Создать файл в корневой дирректории index.js и добавить в него скрипт:
```
const func = () => {
const sum = (a, b) => a + b;
let x = 10;
let y = 20;

console.log(sum(x, y)); // 30
debugger;
x = 20;
y = 30;

console.log(sum(x, y)); // 50
};

func();
```
