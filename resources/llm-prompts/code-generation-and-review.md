# Ограниченная генерация и review кода

Разрешённый объект генерации должен быть назван точно: один method или один class. Передайте package, interfaces, signatures, domain model, dependencies, error policy и готовые acceptance tests.

Явно запретите:

- менять соседние классы и public API;
- добавлять зависимости или скрытые global state;
- генерировать части, отмеченные в КИМ как самостоятельные;
- возвращать пояснения или Markdown, если ожидается содержимое файла.

Для review передайте готовый код и checklist, например: type safety, raw types, unchecked casts, resource handling, SQL injection, timeouts и secret exposure. Требуйте замечания с location, severity и rationale, а не переписанный проект.

Скомпилируйте результат, запустите заранее подготовленные тесты и проверьте diff. Каждую рекомендацию примите или отклоните с обоснованием.
