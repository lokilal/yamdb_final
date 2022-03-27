##### ✨ Груповой проект YaMDb
- Проект YaMDb собирает отзывы (Review) пользователей на произведения (Titles). Произведения делятся на категории: «Книги», «Фильмы», «Музыка».
- Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.
В каждой категории есть произведения: книги, фильмы или музыка. Например, в категории «Книги» могут быть произведения «Винни-Пух и все-все-все» и «Марсианские хроники», а в категории «Музыка» — песня «Давеча» группы «Насекомые» и вторая сюита Баха.
- Произведению может быть присвоен жанр (Genre) из списка предустановленных (например, «Сказка», «Рок» или «Артхаус»). Новые жанры может создавать только администратор.
- Благодарные или возмущённые пользователи оставляют к произведениям текстовые отзывы (Review) и ставят произведению оценку в диапазоне от одного до десяти (целое число); из пользовательских оценок формируется усреднённая оценка произведения — рейтинг (целое число). На одно произведение пользователь может оставить только один отзыв.
##### Чтобы скачать проект к себе на компьютер введите в консоле https://github.com/lokilal/yamdb_final
##### Развернутый проект можно посмотреть здесь ```http://51.250.104.198/```
##### Чтобы запусть проект в консоле введите:
- ``` cd yamdb_final```
- ``` docker-compose up -d ```
- После чего в браузере откройте страницу 
```http://localhost/```
##### Введите в консоль сдедующие команды:
###### Чтобы сделать миграции:
- ``` docker-compose exec web python manage.py migrate --no-input ```
###### Чтобы собрать статику: 
- ``` docker-compose exec web python manage.py collectstatic --no-input ```
###### Чтобы создать суперпользователя: 
- ``` docker-compose exec web python manage.py createsuperuser ```
###### Чтобы загрузить фикстуры: 
- ``` docker-compose exec web python manage.py loaddata fixtures.json ```

##### Created by lokilal 
