# ВБ Банк — МСФО 3М2026

**Work:** `IFRS-WB-2026-3M-01`  
**Тип:** исследование одного отчетного объекта МСФО  
**Статус:** `COMPLETE / NOT_FOUND_UNDER_BOUNDED_SEARCH`  
**Дата отсечения знаний:** 2026-09-16  
**Метод:** `AM-002.2`; `MADARAII/dev@721a199352b5c5282b1478cd6a5eb36a9872fb34`, `FOUNDATION`, `MADARAII-08`, `EXAMPLE-08`

## Результат

В проверенном официальном контуре **не обнаружена самостоятельная промежуточная финансовая отчетность по МСФО ООО «ВБ Банк» за 3 месяца, завершившиеся 31 марта 2026 года**.

Терминальный статус Work — `NOT_FOUND_UNDER_BOUNDED_SEARCH`.

Этот статус означает результат ограниченного поиска. Он не доказывает отсутствие документа во всех возможных каналах и не равен `NOT_PUBLISHED`. Существование конкретного отчета МСФО также не подтверждено, поэтому статус `REPORT_EXISTS_ACCESS_LIMITED` неприменим.

## Reporting entity и reporting lens

Искомый reporting entity:

- полное наименование: **Общество с ограниченной ответственностью «Вайлдберриз Банк»**;
- сокращенное наименование: **ООО «ВБ Банк»**;
- английское наименование: **Wildberries Bank Company Limited; WB Bank**;
- ИНН `0102000578`;
- ОГРН `1020100002340`;
- регистрационный номер Банка России `841`.

Источник идентичности: [карточка участника финансового рынка Банка России](https://www.cbr.ru/finorg/foinfo/?ogrn=1020100002340).

Reporting lens этой Work — **МСФО именно указанного банка**. Отчетность по российским правилам, формы Банка России, раскрытия Wildberries/Russ или иных групп и сегментов не являются заменой искомого объекта.

## Проверенный официальный контур

| Маршрут | Что проверено | Результат |
|---|---|---|
| [ООО «ВБ Банк» — раскрытие информации](https://wb-bank.ru/documents/disclosure) | раздел «Публикуемая отчётность», 2026 год | на странице размещена обобщенная промежуточная бухгалтерская (финансовая) отчетность на 1 апреля 2026 года; отдельный объект МСФО за 3М2026 на странице не идентифицирован |
| [Отчет ВБ Банка на 1 апреля 2026 года](https://wb-bank.ru/documents/generalized_financial_04_05_2026.pdf) | титульный аудиторский блок и база подготовки | аудитор указывает, что отчетность подготовлена по правилам бухгалтерской (финансовой) отчетности, установленным в Российской Федерации; документ относится к российскому отчетному lens и исключен из МСФО-базы |
| [Банк России — отчетность ООО «ВБ Банк»](https://www.cbr.ru/finorg/foinfo/reports/?ogrn=1020100002340) | доступные формы отчетности банка | маршрут содержит регуляторные формы, включая формы 101, 102 и капитал/нормативы; это российская регуляторная отчетность, а не МСФО |
| ЦРКИ Интерфакс / ПРАЙМ, поиск по точным идентификаторам `0102000578` и `1020100002340` | поиск карточки эмитента и attachment МСФО 3М2026 | релевантный документ ВБ Банка в доступном поисковом представлении не локализован; нерелевантные совпадения исключены |
| Поиск по официальному домену `wb-bank.ru` по ключам `МСФО`, `IFRS`, `31 марта 2026`, `3М2026` | дополнительная проверка прямого owner route | отдельный документ МСФО за 3М2026 не обнаружен |

## Граница доказательства

Официальный сайт банка подтверждает наличие отчетности за I квартал 2026 года, но найденный документ относится к российской бухгалтерской отчетности. Его показатели в данный Result не переносятся.

Банк России подтверждает идентичность reporting entity и наличие российской регуляторной отчетности. Эти формы также не используются как финансовая база МСФО.

Поиск не устанавливает факт непубликации МСФО. Допустимая формулировка ограничена состоянием: **документ не найден в проверенном контуре**.

## Следствие для последующего сведения МСФО

Research Work 3М2026 закрыта терминальным отрицательным результатом. Для сведения ВБ Банка этот Result должен входить в source universe как ограничение:

- отчетная точка МСФО 3М2026 отсутствует в доступной доказательной базе;
- российская отчетность и регуляторные формы не заменяют этот пробел;
- чистый II квартал по накопленным показателям МСФО нельзя рассчитывать вычитанием из 6М2026 без совместимой точки 3М2026;
- показатели 3М2026 по МСФО сохраняются как `UNKNOWN`.

## Completion record

```yaml
scope_boundary: standalone IFRS reporting object of ООО «ВБ Банк» for 3M2026
reporting_entity: ООО «ВБ Банк» / Общество с ограниченной ответственностью «Вайлдберриз Банк»
reporting_lens: IFRS of the exact bank entity
material_period: 2026-01-01..2026-03-31
terminal_status: NOT_FOUND_UNDER_BOUNDED_SEARCH
coverage:
  bank_official_disclosure_route: checked
  bank_q1_2026_published_statement: checked_wrong_lens_RAS
  bank_of_russia_entity_and_reporting_route: checked_wrong_lens_regulatory
  exact_identifier_disclosure_search: checked_no_relevant_ifrs_attachment_found
  official_domain_ifrs_keyword_search: checked_no_relevant_ifrs_attachment_found
material_unknowns:
  - existence and locator of a standalone IFRS report for 3M2026 outside the checked contour
reliance_envelope: terminal negative Research Result; no IFRS financial metrics established
stop_basis:
  - principal official bank disclosure route checked
  - Bank of Russia reporting route checked and separated by lens
  - exact-identifier disclosure search checked
  - further search had low expected value within the commissioned bounded official contour
reopen_rule: only a separate direct user command may reopen this completed Work
```
