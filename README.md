Генератор текстов писателя В.О. Пелевина с использованием реккурентных нейросетей (RNN)

Содержит три модуля:
1. Препроцессинг текста
Обрабатывает текст, чистит от ненужных символов, обрезает предложения для подачи в нейросеть и составляет словарь токенов
!!! требует исходные тексты книг в формате txt !!!

2. Тренировочный модуль
Определяет нейросеть, тренирует в цикле на GPU (необходимо около 5Gb видеопамяти). Сохраняет итоговые веса в файл.
!!! требует исходные тексты книг в формате txt !!!

3. Генератор текста
Загружает веса из файла в нейросеть и генерирует текст. По умолчанию используется предобученная мною сеть с весами из файла 'model.lol'


Некоторые вспомогательные функции взяты из курса "Нейронные сети и обработка текста" на Stepik.
