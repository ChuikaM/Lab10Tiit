# Пример README.md

Этот файл демонстрирует базовый синтаксис Markdown.

## 1. Форматирование текста

- **Полужирный текст**
- *Курсив*
- ~~Зачёркнутый текст~~
- ***Полужирный курсив***
- `Моноширинный текст`

## 2. Списки

### Ненумерованный список
- Элемент 1
- Элемент 2
  - Вложенный элемент (добавляется 2 пробела)
- Элемент 3

### Нумерованный список
1. Первый пункт
2. Второй пункт
   1. Вложенный пункт
3. Третий пункт

## 3. Подзаголовки разного уровня

# Заголовок 1 уровня (`#`)
## Заголовок 2 уровня (`##`)
### Заголовок 3 уровня (`###`)
#### Заголовок 4 уровня (`####`)

## 4. Ссылки

- [Google](https://www.google.com)
- [GitHub](https://github.com)

## 5. Изображения

![Логотип GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
![Пример изображения](hl2_logo.png)

## 6. Пример кода

### Пример исходного кода C++ SFML
```cpp
#include <SFML/Graphics.hpp>

int main()
{
    sf::RenderWindow window(sf::VideoMode({200, 200}), "SFML works!");
    sf::CircleShape shape(100.f);
    shape.setFillColor(sf::Color::Green);

    while (window.isOpen())
    {
        while (const std::optional event = window.pollEvent())
        {
            if (event->is<sf::Event::Closed>())
                window.close();
        }

        window.clear();
        window.draw(shape);
        window.display();
    }
}
```