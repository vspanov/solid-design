Минимум:
1. Внедрите Ninject container для создания Program. (см. метод Program.Main)

Основная программа:
2. Добавьте команду HelpCommand, печатающую список всех доступных команд (в том числе себя). Для этого придется побороть циклическую зависимость.
3. Сделайте явной зависимость от TextWriter и используйте его, вместо консоли и в командах, и в Program.

Дополнительно:
4. Попробуйте подход Convention over configuration в Ninject. Для этого изучите extension-метод Bind(c => ...) из пространства имен Ninject.Conventions.
5. Биндить что-то на TextWriter — не очень хорошая идея. TextWriter — это слишком общая штука.
Примените идею именованных зависимостей в Ninject (атрибут Named), чтобы избавиться от этой проблемы.
