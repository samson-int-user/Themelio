# Особенности браузеров

## Переносы слов

[Поддержка](http://caniuse.com/css-hyphens)

ФФ24 не расставляет переносы автоматически, если у тега `html` не указан атрибут `lang` со значением, соответствующим языку текста, в котором требуется расставлять переносы. Таким образом, если на странице есть тексты на разных языках, разработчику следует выбрать язык, текст на котором будет оформлен переносами.

ИЕ10 основывается на языке системы. (?) !!!Проверить в виртуальной машине.


## Тень элемента

[Поддержка](http://caniuse.com/css-boxshadow)

[Нельзя просто так взять и нарисовать одинаковую тень!](https://twitter.com/Ser_Gen/status/359736688269987840)

[Тест](http://jsfiddle.net/SerGen/G8grk/)

Отрисовка тени в различных браузерах столько же значительно отличается.
Самая маленькая тень отрисовывается Хромом, самая большая — ФФ. Ближе к правильным значениям Опера 12.


## Трансформации

[Поддержка](http://caniuse.com/transforms2d)

[Некоторые браузеры отказываются одинаково трансформировать элементы](https://twitter.com/Ser_Gen/status/359728485750669313)

[Тест](http://jsfiddle.net/SerGen/XUyVK/)

Лучше всего отображение в ФФ.


## Переходы

[Возможно, кому-то ещё встретится такая проблема (проявляется только в ФФ)](https://twitter.com/Ser_Gen/status/354889748789215232)

Не срабатывает анимация-переход, если у элемента-родителя изменяется [способ позиционирования](http://jsfiddle.net/jCfwc/) или [поведение при переполнении](http://jsbin.com/eZOsEja/3/edit).

[Древний баг на трекере ФФ](https://bugzilla.mozilla.org/show_bug.cgi?id=625289)
