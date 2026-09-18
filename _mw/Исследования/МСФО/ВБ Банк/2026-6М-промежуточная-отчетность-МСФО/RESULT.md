# ВБ Банк — МСФО 6М2026

**Work:** `IFRS-WB-2026-6M-01`  
**Тип:** исследование одного отчетного объекта МСФО  
**Статус:** `COMPLETE / NOT_FOUND_UNDER_BOUNDED_SEARCH`  
**Дата отсечения знаний:** 2026-09-16  
**Метод:** `AM-002.2`; `MADARAII/dev@721a199352b5c5282b1478cd6a5eb36a9872fb34`, `FOUNDATION`, `MADARAII-08`, `EXAMPLE-08`

## Результат

В проверенном официальном контуре **самостоятельная промежуточная финансовая отчетность по МСФО ООО «ВБ Банк» за шесть месяцев, завершившихся 30 июня 2026 года, не обнаружена**.

Терминальный статус Work — `NOT_FOUND_UNDER_BOUNDED_SEARCH`.

Статус описывает результат ограниченного поиска. Он не доказывает отсутствие документа во всех возможных каналах и не равен `NOT_PUBLISHED`. Существование конкретного отчета МСФО за 6М2026 также не подтверждено, поэтому статус `REPORT_EXISTS_ACCESS_LIMITED` неприменим.

## Reporting entity и reporting lens

Reporting entity сохраняется тем же, что в завершенной Work 3М2026:

- полное наименование: **Общество с ограниченной ответственностью «Вайлдберриз Банк»**;
- сокращенное наименование: **ООО «ВБ Банк»**;
- английское наименование: **Wildberries Bank Company Limited; WB Bank**;
- ИНН `0102000578`;
- ОГРН `1020100002340`;
- регистрационный номер Банка России `841`.

Источник идентичности: https://www.cbr.ru/finorg/foinfo/?ogrn=1020100002340

Reporting lens этой Work — **МСФО указанного банка**. Российская бухгалтерская отчетность, формы Банка России, регуляторные раскрытия, отчетность Wildberries/Russ и иных групп или сегментов не заменяют искомый объект.

Материальный период — `2026-01-01..2026-06-30`; целевая отчетная точка — конец первого полугодия 2026 года.

## Проверенный официальный контур

| Маршрут | Что проверено | Результат |
|---|---|---|
| https://wb-bank.ru/documents/disclosure | раздел «Публикуемая отчётность», 2026 год | на странице указаны обобщенная промежуточная бухгалтерская (финансовая) отчетность на 1 июля 2026 года и аналогичный объект на 1 апреля 2026 года; отдельный объект МСФО за 6М2026 не идентифицирован |
| https://wb-bank.ru/documents/generalized_financial_03_08_2026.pdf | официальный полугодовой документ банка, размещенный 03.08.2026 | аудитор указывает, что исходная промежуточная бухгалтерская (финансовая) отчетность за первое полугодие 2026 года подготовлена по правилам, установленным в Российской Федерации; пакет включает публикуемые формы 0409806, 0409807 и другие российские формы; документ относится к другому reporting lens |
| https://www.cbr.ru/finorg/foinfo/?ogrn=1020100002340 | карточка участника финансового рынка | подтверждены идентичность reporting entity, ИНН, ОГРН и рег. № 841 |
| https://www.cbr.ru/finorg/foinfo/reports/?ogrn=1020100002340 | отчетность банка в контуре Банка России | доступны российские регуляторные формы, включая форму 101 и другие отчетные точки; самостоятельный объект МСФО в этом маршруте не установлен |
| поиск по официальному домену `wb-bank.ru` по сочетаниям `МСФО`, `IFRS`, `30 июня 2026`, `6М2026`, `WB Bank`, `Вайлдберриз Банк` | дополнительная проверка owner route | отдельный отчет МСФО за 6М2026 не обнаружен |
| поиск по точным идентификаторам `0102000578` и `1020100002340` с ключами `МСФО` / `IFRS` | дополнительная проверка публичной индексируемости | конкретный standalone-отчет МСФО за 6М2026 не локализован |

## Граница доказательства

Официальная страница раскрытия подтверждает публикацию полугодового финансового документа банка, однако сам документ прямо задает российскую основу составления. Это надежно исключает его использование как МСФО выбранного reporting entity.

Финансовые показатели из данного российского отчета, форм Банка России и иных reporting lenses в этот Result не переносятся.

Поиск не устанавливает факт непубликации МСФО. Допустимая формулировка ограничена состоянием: **standalone-документ МСФО за 6М2026 не найден в проверенном контуре**.

Остается `UNKNOWN` существование непубличной, неиндексируемой либо размещенной вне проверенного контура самостоятельной МСФО ООО «ВБ Банк» за 6М2026.

## Следствие для последующего сведения МСФО

Research Work 6М2026 закрыта терминальным отрицательным результатом. При последующем сведении ВБ Банка этот Result должен использоваться только как ограничение source universe:

- отчетная точка МСФО 6М2026 отсутствует в доступной доказательной базе;
- российская отчетность и регуляторные формы этот пробел не заменяют;
- финансовые показатели 6М2026 по МСФО сохраняются как `UNKNOWN`;
- вместе с терминальным отрицательным Result 3М2026 доступная база не позволяет получить чистый II квартал по МСФО.

## Completion record

```yaml
scope_boundary: standalone IFRS reporting object of ООО «ВБ Банк» for 6M2026
reporting_entity: ООО «ВБ Банк» / Общество с ограниченной ответственностью «Вайлдберриз Банк»
reporting_lens: IFRS of the exact bank entity
material_period: 2026-01-01..2026-06-30
terminal_status: NOT_FOUND_UNDER_BOUNDED_SEARCH
coverage:
  bank_official_disclosure_route: checked
  bank_h1_2026_published_statement: checked_wrong_lens_Russian_accounting
  bank_of_russia_entity_route: checked
  bank_of_russia_reporting_route: checked_wrong_lens_regulatory
  official_domain_ifrs_keyword_search: checked_no_relevant_ifrs_object_found
  exact_identifier_public_search: checked_no_specific_ifrs_report_found
material_unknowns:
  - existence and locator of a standalone IFRS report for 6M2026 outside the checked contour
residual_risks:
  - a non-indexed or non-public IFRS object could exist outside the bounded search universe
reliance_envelope: terminal negative Research Result; no IFRS financial metrics established
stop_basis:
  - principal official bank disclosure route checked
  - the published H1 document was inspected and identified as Russian accounting rather than IFRS
  - Bank of Russia entity and reporting routes checked and separated by lens
  - exact-identifier and official-domain searches did not locate a specific IFRS object
  - further search had low expected value within the commissioned bounded contour
reopen_rule: only a separate direct user command may reopen this completed Work
```
