Привет. Я разработчик и менеджер. Пишу и код и тексты. И я страдал.

Думаю вам знакома проблема изменения расположения спецсимволов в зависимости от раскладки. В 2023 году в русские тексты пришли символы с английской раскладки, такие как #, $, @. Чтобы их набирать приходится менять раскладку туда-сюда. Это не удобно.

Все изменилось, когда я сделал свою раскладку. Она реально удобная для всех русскоязычных айтишников.

## Основные фишки
1. Одинаковый набор популярных спецсимволов по «Shift + цифра» независимо от языка. Теперь можно печатать #хештеги и @меншены не меняя язык! Ради этого все и делалось на самом деле.
2. Менее популярные не пропали, а скрыты под «Alt + цифра».
3. Базово везде установлен «/», «|» и «\» доступны по Shift или Alt одинаково на обоих языках.
4. На «<» и «>» с модификатором Alt печатаются нормальные кавычки-елочки: «». Ваш текст сразу станет лучше.
5. На «-» с модификатором Alt доступен символ длинное тире «—».

extra! Так же добавил конфиг правила для Karabiner для удобного переключения:
- По нажатию на правый Command — английская раскладка
- По нажатию на левый Command — русская раскладка

Теперь не нужно думать какая раскладка включена. Просто перед набором жмешь нужный Command и печатаешь без ошибок.

## Слои

https://github.com/StipJey/SJKL/assets/8746529/fac22ca0-2b67-49ff-9107-ce50266f611d


https://github.com/StipJey/SJKL/assets/8746529/5520ee64-046e-415b-80e1-b8b245db1f60


## Инструкция
### Установка раскладки
0. Зайдите в [релизы](https://github.com/StipJey/SJKL/releases) и скачайте актуальный SJKL.dmg
1. Запустите SJKL.dmg
2. Запустите Keyboard Installer
3. Перетащите файл SJKL.bundle в окно Keyboard Installer'а
4. Нажмите на Install for current user (recommended)
5. Перезагрузите компьютер или завершите сеанс
6. Зайдите в Настройки → Клавиатура → Источники ввода → Изменить
7. Нажмите на «+» в левом нижнем углу открывшегося окна
8. Выберете в разделе русских раскладок «Русская — SJKL»
9. Выберете в разделе английских раскладок «English — SJKL»
10. Удалите все лишние раскладки, нажав на «-», если он доступен

У вас может не удалиться стандартная английская раскладка, это баг свежей MacOs. На старых версиях можно было добавить Японскую и тогда у английской появлялся «-». Если вы знаете как удалить лишнюю раскладку, пожалуйста, создайте ишью с описанием механизма.
 
### Установка скрипта в Karabiner
1. Поставьте и запустите карабинер.
2. Откройте Finder
3. Нажмите на Command + Shift + G
4. В строку вставьте адрес: `~/.config/karabiner/assets/complex_modifications/`
5. Скопируйте в открывшуюся папку файл [karabiner-rule.json](karabiner-rule.json)
6. В карабинере перейдите на вкладку Complex Modifications
7. Нажмите на кнопку «Add rule»
8. В открывшемся окне нажмите на кнопку Enable у модификатора «Change input source to SJKL (RU) by left_command; SJKL (EN) by right_command»

### Готово

Теперь у вас доступны все ништяки раскладки, осталось только привыкнуть.
Приятного использования!

## Планы
1. Продумать слой под Alt. В него можно добавить много классных символов, в том числе и смайлики. Пишите ваши предложения в Issues.

## Вдохновение и благодарность

Я сделал раскладку на основе идей из двух раскладок:
1. [Strata Markdown ](https://github.com/Atarity/Strata/tree/master)
2. [Ручей (Ruchey) ](https://github.com/a-projects/ruchey)

В Страте решен вопрос с наличием символов для удобного набора текстов. Под рукой нормальные кавычки « », длинное тире —, стрелочки ← → и прочие символы.
У Ручья отличная идея с фиксированным расположением независимо от раскладки, но она ппц какая неудобная для меня.

Стратой я пользовался несколько лет, но решил что пора объединить эти две идеи и сделал свой микс

Благодарю создателей этих раскладок.

Благодарю свою жену, за то что дала возможность посвятить время этому проекту.

А поблагодарить меня можно через донат любой суммы по ссылке: https://stipjey.taplink.ws/
Там же ссылки на другие мои продукты и проекты.
