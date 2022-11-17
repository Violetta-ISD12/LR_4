��#� �L�R�_�4�
Як виконати відправку закомічених змін на сервер?
git push

Як виконати затягування змін із сервера?
git pull

Як проводиться синхронізація робочої копії із затягнутими змінами?
git merge

Як проводиться синхронізація робочої копії із затягнутими змінами для проекта з під модулями?
git submodule update --remote

Де зберігаються файли при використанні розподіленої системи контролю версій?
.git/remote

Які переваги дає використання розподіленої системи контролю версій?
Створення різних версій файлів. Можливість працювати над одним проектом разом, без незручності ручного синхронізування. Створення логу коммітів якщо хтось зламав прод, то його можна побити.

Які недоліки має використання розподіленої системи контролю версій?
Відсутність можливості заблокувати файли, але це можно обійти за допомогою захищенних гілок і автоматичного тестування коду. В публічний репозиторій будь їто може додати код, якщо неправильно налаштований, або аккаунт людини с доступом був скомпрометований.

Що таке репозиторій?
Магічна "папка", яка зберігае як відомості про зміну файлів, так і їх поточну версію.

Навіщо потрібні розподілені системи?
Для зручною роботи над проектом командою розробників.

Що таке оновлення робочої копії проекту?
У міру внесення змін в основну версію проекту робоча копія на комп'ютері розробника старіє: розбіжність її з основною версією проекту збільшується. Це підвищує ризик виникнення конфліктних змін. Тому зручно підтримувати робочу копію в стані, максимально близькому до поточної основної версії, для чого розробник виконує операцію поновлення робочої копії (update) наскільки можливо часто (реальна частота оновлень визначається частотою внесення змін, залежної від активності розробки і числа розробників, а також часом, затрачуваним на кожне оновлення - якщо воно велике, розробник змушений обмежувати частоту оновлень, щоб не втрачати час).

Що таке фіксація змін проекту?
Завершивши черговий етап роботи над завданням, розробник фіксує (commit) свої зміни, передаючи їх на сервер (або в основну гілку, якщо робота над завданням повністю завершена, або в окрему гілку розробки даного завдання).

Що таке модифікація проекту?
Модифікація проекту Розробник модифікує проект, змінюючи вхідні в нього файли в робочій копії відповідно до проектним завданням. Ця робота проводиться локально і не вимагає звернень до сервера СКВ.

Для чого використовується розгалуження в СКВ?
Гілки використовують для зберігання незавершених, експерементальних та повністю готових версій проєкту.

Що таке «Злиття версій»?
Злиття всіх поточніх розробок у проекті для формування релізної версії.

Що розуміють під конфліктом при роботі СКВ?
Конфлікт версій вмісту файла. Зазвичай це стаеться через те що файл був змінений різними розробниками і СКВ не знає яку версію файла використовувати.

За яких умов злиття версій проходить автоматично і без конфліктів?
Коли немає ніяких змін у файлі в одній з гілок.

Чи призводить видалення та зміна одного і того ж файлу або каталогу у різних версіях до конфлікту при їх злитті?
Так, СКВ не буде знати яку версію файла використовувати. Такі конфлікти повинні вирішуватись розробником.
