# Хакатон Банк России
RAG system with LLM

Модель эмбедингов: intfloat/multilingual-e5-large-instruct<br>
Протестированные LLM: ai-forever/FRED-T5-1.7B  и IlyaGusev/saiga_mistral_7b_lora<br>
Векторная БД: ChromaDB
# Решение:
Файл [CBhack_with_dataset.ipynb](https://github.com/PocketBrain/CB_Hack/blob/main/CBhack_with_dataset.ipynb) - содержить полный пайплайн с созданием эмбедингов и препроцессинга данных. <br>
Файл [ResultLLM.ipynb](https://github.com/PocketBrain/CB_Hack/blob/main/ResultLLM.ipynb) - Используется для работы, при наличие файла эмбедингов.<br>
GIT [Telegram Bot](https://github.com/Cirilus/PurpleTgBot)- <br>
URL [Telegram Bor](https://t.me/CBR_supportBot) - Для запуска и демонстрации работы RAG<br>
# Фичи:
1)Кастомная рекурсивная разбивка данных на чанки(блоки) с помощью регулярных выражений, с большим пересечением чанков.<br>
2)Добавление метаданных к блокам данных: Название файла и страница файла.<br>
3)Использование реранжирования и топ 3 запросов с анализом threshold, для каждого запроса.<br>
4)Использование перефразирования запроса пользователя для создания лучшего промпта.<br>
5)Использование системных токенов в промпте для меньших галюцинаций.<br>
# Датасет:
[https://drive.google.com/file/d/1NzfE5YRHSdpc2rfDKxnBqyKKVpiJjXil/view?usp=drive_link ](https://drive.google.com/file/d/1NzfE5YRHSdpc2rfDKxnBqyKKVpiJjXil/view?usp=sharing)<br>
Датасет был собран с помощью парсинга сайта ЦБ, данные сканов были удалены и взята только потенциально полезная информация для RAG.<br>
https://drive.google.com/file/d/1ixXtR-_JCipCJeTekcwVY5SUfWHOtk_H/view?usp=sharing  - Архив эмбедингов, в случае запуска через ноутбук
