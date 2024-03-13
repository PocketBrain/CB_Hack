# CB_Hack
RAG system with LLM

Модель эмбедингов: intfloat/multilingual-e5-large-instruct<br>
Протестированные LLM: ai-forever/FRED-T5-1.7B  и IlyaGusev/saiga_mistral_7b_lora<br>
Векторная БД: ChromaDB
# Фичи:
1)Кастомная рекурсивная разбивка данных на чанки(блоки) с помощью регулярных выражений, с большим пересечением чанков.<br>
2)Добавление метаданных к блокам данных: Название файла и страница файла.<br>
3)Использование реранжирования и топ 3 запросов с анализом threshold, для каждого запроса.<br>
4)Использование перефразирования запроса пользователя для создания лучшего промпта.<br>
5)Использование системных токенов в промпте для меньших галюцинаций.<br>
