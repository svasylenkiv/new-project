Як зробити Smart Commit крок за кроком:
1. Дізнайся ключ задачі
Задача в Jira має ключ, наприклад: PROJ-123

2. Сформуй коміт

```bash
git checkout development
```
```bash
git add .
```
```bash
git commit -m "PROJ-123 #comment Зробив першу частину задачі #time 2h #transition In Review"
```

Пояснення:
PROJ-123 — ключ Jira задачі

#comment Зробив першу частину задачі — додасть коментар у Jira

#time 2h — залогує 2 години в Jira

#transition In Review — змінить статус задачі на In Review

Назва статусу (In Review) має відповідати точно тому, як названо у Jira.

3. Відправ коміт на сервер

```bash
git push origin development
```

Приклад короткого коміту:
```bash
git commit -m "PROJ-123 #comment Готово #time 1h"
```
