# Submission

Заполните файл перед отправкой PR.

## Ссылка на репозиторий с заданием

- Repo URL: https://github.com/mukhametzyanova27-coder/learn-rag

## Автор

- ФИО: Мухаметзянова Дильбар Ильгизовна
- ник: mukhametzyanova27-coder
- 1 курс магистратуры, группа БАСБ252

## Комментарий

RAG повторён на описаниях пакетов PyPI. Источник: список топ-пакетов hugovk/top-pypi-packages
+ публичный JSON API PyPI; сбор воспроизвожу (scripts/prepare_datasets.py).

- 448 записей в datasets.json → 1920 чанков после нарезки.
- Полный pipeline: ingest → chunking → TF-IDF index → retrieval → demo-answer → Streamlit UI.
- 3 demo-вопроса с ответами и источниками + 1 negative с корректным отказом.
- 12 тестов pytest (green), включая собственный тест на биграммы.
- Улучшение реализовано: TF-IDF ngram_range=(1,2) + sublinear_tf + min_df=2 (см. homework/IMPROVEMENTS.md).
