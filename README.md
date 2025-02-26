# RuSentNE-2023: Соревнование по анализу тональности к именованным сущностям в новостных текстах

### [Ссылка на соревнования в системе Codalab](https://codalab.lisn.upsaclay.fr/competitions/9538)
### [Таблица результатов](https://codalab.lisn.upsaclay.fr/competitions/9538#results)

## Описание:

Анализ тональности текста — извлечение выраженной в тексте эмоциональной оценки к некоторой сущности — одно из наиболее активно развивающихся направлений в автоматической обработке текстов. 

Анализ тональности новостных текстов — важное направление в области анализа мнений, поскольку обнаружение, отслеживание трендов тональности в новостном потоке важно для построения разного рода аналитических систем, отслеживания имиджа в СМИ конкретных людей или компаний. 

## Тональность по отношению к сущности в новостном тексте может происходить по крайней мере из трёх разных источников:
* мнения автора текста,
* цитируемого мнения, при этом сам носитель мнения может быть упомянут или не упомянут в тексте,
* имплицитного мнения, которое следует из каких-либо упомянутых действий или реакций, например, X уволил Y. Такая информация часто присутствует даже при внешне нейтральном изложении событий.
    
Участникам предлагается задача извлечения из новостных текстов тональности трёх классов (негативная, позитивная, нейтральная) по отношению к заранее размеченным сущностям типа PERSON, ORGANIZATION, PROFESSION, COUNTRY, NATIONALITY в рамках отдельного предложения.

## Базовый подход:
* `baseline_submission.zip` -- применение классификатора на основе модели [RuBERT](https://huggingface.co/DeepPavlov/rubert-base-cased) взятой в исходном состоянии.

## Описание данных:
* `sentence` - предложение
* `entity` - объект анализа тональности
* `entity_tag` - тип сущности в рамках PERSON, ORGANIZATION, PROFESSION, COUNTRY, NATIONALITY
* `label` - метка тональности (0 - нейтрально, - 1 - отрицательно, 1 - положительно)

## График проведения соревнования:
* 15 декабря — публикация обучающих данных;
* 15 февраля — публикация тестовых данных;
* 28 февраля — подведение итогов соревнования;
* 25 марта — подача статей.

## Организаторы:
* Лукашевич Н.В. (МГУ им. М.В. Ломоносова)
* Голубев А.А. (МГУ им. М.В. Ломоносова)
* [Русначенко Н.Л.](https://nicolay-r.github.io/) (Newcastle University)

## Ссылки:

[**Codalab:** Named Entity Oriented Sentiment Analysis Task (RuSentNE-2023)](https://codalab.lisn.upsaclay.fr/competitions/9538)

## Источники:

[Официальная страница задачи RuSentNE на сайте Dialogue-2023](https://www.dialog-21.ru/evaluation/2023/rusentne/)

[Официальная информация по конференции Dialogue-2023](https://www.dialog-21.ru/information2023/)
