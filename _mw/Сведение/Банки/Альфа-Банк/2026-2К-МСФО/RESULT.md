# Сведение МСФО — Альфа-Банк, II квартал 2026 года

**Work ID:** `SYNTH-IFRS-ALFA-2026-Q2-01`  
**Тип Work:** `RESEARCH_CORPUS_SYNTHESIS` / MADARAII-10  
**Статус:** завершено  
**Reporting entity:** Группа АО «АЛЬФА-БАНК»  
**Reporting lens:** консолидированная отчетность по МСФО  
**Материальный период:** II квартал 2026 года; отчетная дата 30.06.2026; 6М2026 используется как накопленный отчетный период  
**Дата отсечения знаний:** 2026-09-16  
**Инженерная основа:** `MADARAII/dev@721a199352b5c5282b1478cd6a5eb36a9872fb34`, `FOUNDATION`, `MADARAII-10`, `EXAMPLE-10`  
**Аналитическая основа:** `AM-002.2`, `PROFILE-BANKING`, `METHOD-COMPARE`, `METHOD-DECOMPOSE`  

## 1. Граница и source universe

Сведение построено только по двум завершенным Research Results текущего МСФО-контура Альфа-Банка:

1. `Исследования/МСФО/Альфа-Банк/2026-3М-промежуточная-консолидированная-отчетность/RESULT.md` — `IFRS-ALFA-2026-3M-01`, статус `REPORT_EXISTS_ACCESS_LIMITED`;
2. `Исследования/МСФО/Альфа-Банк/2026-6М-промежуточная-консолидированная-отчетность/RESULT.md` — `IFRS-ALFA-2026-6M-01`, завершенный Result в ограниченном контуре доступной доказательной базы.

Baseline источников: blobs `740b91acb90b06e66bea501b61dd47c381c68cf3` и `cbd12a019c08dedc5abe20e7f5b6df253f7b4360`.

РСБУ, формы Банка России, новости, сектор, макроэкономика, другие банки и новый внешний Research в source universe отсутствуют.

Research Result 3М2026 подтверждает существование отчетного объекта и установленный reporting perimeter, но числовой базы первичной МСФО в нем нет. Research Result 6М2026 содержит накопленные 6М-показатели, балансовые точки 31.03/30.06 и ряд clean-Q2 значений, уже рассчитанных либо прямо подтвержденных внутри этой Research Work. В настоящем сведении такие clean-Q2 значения сохраняются как **унаследованные `derived`-наблюдения 6М Result**. Новый расчет `6М − 3М` по двум Research Results здесь отсутствует, поскольку 3М Result не содержит числовых входов.

## 2. Primary Analytical Result

### 2.1. Прибыль: сильные 6М скрывают резкое замедление во II квартале

Чистая прибыль группы за 6М2026 составила **186,9 млрд руб.**, +57,5% г/г. Унаследованный clean Q2 из 6М Result — **82,5 млрд руб.**; прямой secondary headline — **82,6 млрд руб.** Это около **-20,9% кв/кв** и примерно **+0,5–1% г/г**.

Основной вывод периода: полугодовой темп прибыли сформирован в значительной степени I кварталом. II квартал показывает почти неизменную прибыль год к году при заметном снижении относительно I квартала.

### 2.2. Процентный результат усилился быстрее итоговой прибыли

NII до резервов за 6М2026 — **413,1 млрд руб.** Унаследованный clean Q2 — **213,7 млрд руб.**, около **+7,2% кв/кв** и **+31,0% г/г**.

Процентные доходы clean Q2 — **552,1 млрд руб.**, около **+0,1% кв/кв** и **+2,5% г/г**. Следовательно, рост NII существенно опередил динамику gross interest income. Это механическое наблюдение о P&L-структуре. Декомпозиция на repricing, стоимость фондирования и mix остается `UNKNOWN` без полного набора примечаний и средних балансов.

При этом OPEX во II квартале составил **97,1 млрд руб.**, +37% г/г. ECL headline — **47,7 млрд руб.**, около -23% г/г. Рост NII и снижение risk-flow не перешли в сопоставимый рост чистой прибыли: часть эффекта поглощена расходами и иными P&L-компонентами, точный bridge остается `UNKNOWN`.

### 2.3. Баланс расширился через ликвидность и клиентское фондирование

На 30.06.2026 активы достигли **14,39 трлн руб.**, +6,5% к 31.03.2026. Квартальный рост активов составил около **882 млрд руб.** и почти совпал с приростом денежных средств и эквивалентов — около **844 млрд руб.**

Одновременно:

- денежные средства и эквиваленты выросли с **489,8 млрд** до **1 334,0 млрд руб.**;
- net loans / net lease investments снизились с **9,42 трлн** до **9,32 трлн руб.**, около -1,1% кв/кв;
- gross credit portfolio снизился с **9,86 трлн** до **9,75 трлн руб.**, около -1,1% кв/кв;
- средства клиентов выросли с **9,65 трлн** до **10,45 трлн руб.**, около +8,4% кв/кв;
- капитал вырос с **1,31 трлн** до **1,34 трлн руб.**

Это поддерживает `MECHANICAL_L1`-вывод: расширение баланса во II квартале было преимущественно ликвидным, при росте клиентского фондирования и сокращении кредитного book. Экономическая причина накопления ликвидности остается за пределами доступной МСФО-базы.

### 2.4. Качество book по 90+ умеренно ухудшилось

В доступном определении 90+:

- 90+ / gross loans: **2,91%** на 30.06.2026 против **2,87%** на 31.03.2026 и **2,70%** на 31.12.2025;
- reserve / gross loans: **4,40%** против **4,41%** кварталом ранее;
- reserve / 90+ coverage: **151%** против **153%** кварталом ранее и **163%** на конец 2025 года.

Картина указывает на постепенный рост доли 90+ при стабильном общем резервировании к gross book и снижении покрытия 90+. Конструкции Stage 3, NPL90 и 90+ сохраняются раздельно; bank-reported Stage 3 остается `UNKNOWN`.

### 2.5. Периметр группы ограничивает годовую сопоставимость

Сделка по приобретению 87,5% «Европлана» закрыта в декабре 2025 года, и 6М2026 уже относятся к группе с контролируемым лизинговым бизнесом. Поэтому годовые сравнения 2026/2025 потенциально включают эффект изменения консолидационного периметра.

Точный organic/perimeter bridge отсутствует. Рост активов, доходов, расходов и прибыли г/г следует трактовать с учетом этой границы сопоставимости.

## 3. Reconciled evidence table

Все суммы — млрд руб., если не указано иное.

### 3.1. Stocks и ratios

| Показатель | 31.03.2026 | 30.06.2026 | Изменение / статус |
|---|---:|---:|---|
| Активы | 13 510,0 | 14 392,2 | +882,2; +6,5% кв/кв; reported-secondary в 6М Result |
| Cash & equivalents | 489,8 | 1 334,0 | +844,2; reported-secondary |
| Net loans / net lease investments | 9 422,2 | 9 320,5 | -101,7; около -1,1% |
| Gross credit portfolio | 9 856,8 | 9 749,4 | -107,4; около -1,1% |
| Средства клиентов | 9 647,8 | 10 453,5 | +805,7; около +8,4% |
| Обязательства | 12 204,8 | 13 048,1 | +843,3 |
| Капитал | 1 305,2 | 1 344,1 | +38,9 |
| Net loans / customer funds | 97,66% | 89,16% | derived; снижение funding pressure proxy |
| Reserve / gross loans | 4,41% | 4,40% | derived; практически стабильно |
| 90+ / gross loans | 2,87% | 2,91% | derived; умеренный рост |
| Reserve / 90+ | 153% | 151% | derived; снижение |

### 3.2. Flows

| Показатель | 6М2026 | Clean Q2 2026 | Q2 динамика | Статус |
|---|---:|---:|---|---|
| Процентные доходы | 1 103,5 | 552,1 | +0,1% кв/кв; +2,5% г/г | 6М secondary; Q2 inherited derived |
| NII до резервов | 413,1 | 213,7 | +7,2% кв/кв; +31,0% г/г | 6М secondary; Q2 inherited derived и direct-secondary confirmed |
| Чистые комиссионные доходы | 70,1 | 37,2 | г/г `UNKNOWN` | inherited derived |
| Прибыль до налога | 235,9 | 108,2 | -15,3% кв/кв; +4,6% г/г | inherited derived |
| Чистая прибыль | 186,9 | 82,5–82,6 | -20,9% кв/кв; около +0,5–1% г/г | 82,5 inherited derived; 82,6 direct-secondary headline |
| ECL / резервный расход | `UNKNOWN` в полной сопоставимой 6М-строке | 47,7 | около -23% г/г | direct-secondary Q2 headline; конфликт охвата сохраняется |
| OPEX | `UNKNOWN` в полной накопленной строке | 97,1 | +37% г/г | direct-secondary Q2 headline |

## 4. Конфликты, зависимости и ограничения

1. **3М source gap.** 3М Result терминально подтверждает существование отчета, но содержит нулевой числовой payload первичной МСФО. Поэтому самостоятельный пересчет clean Q2 из пары Research Results отсутствует.
2. **Clean-Q2 lineage.** Числа clean Q2 выше унаследованы из 6М Result. Их статус остается `derived` либо `direct-secondary`, как зафиксировано исходной Research Work.
3. **Общая линия происхождения вторичных источников.** Несколько публикаций 6М Result транслируют одну базовую отчетность. Число реплик не считается независимой бухгалтерской верификацией.
4. **NII definition.** Значение **314,8 млрд руб.** в Cbonds описано как NII после резервов и остается отдельной конструкцией от NII до резервов **413,1 млрд руб.**
5. **ECL scope conflict.** Прямой Q2 headline **47,7 млрд руб.** расходится с арифметически implied разницей около **41,0 млрд руб.** между двумя Cbonds-строками. Охват показателей остается `UNKNOWN`.
6. **90+ и Stage 3.** Доля 90+ подтверждает динамику только соответствующего construct. Stage 3/NPL и официальное coverage остаются отдельными `UNKNOWN`.
7. **M&A/perimeter.** Сравнение г/г включает риск изменения периметра после консолидации «Европлана». Organic growth без purchase-accounting bridge остается `UNKNOWN`.
8. **Primary attachment access.** Точные primary attachments 3М2026 и 6М2026 отсутствуют в доступном контуре исходных Research Results. Это ограничивает note-level анализ и bank-reported KPI.

## 5. Материальные UNKNOWN

| Блок | Статус |
|---|---|
| Bank-reported NIM | `UNKNOWN` |
| Bank-reported CIR | `UNKNOWN` |
| Bank-reported CoR | `UNKNOWN` |
| Stage 2 / Stage 3 и официальное NPL coverage | `UNKNOWN` |
| Regulatory capital / RWA | `UNKNOWN` |
| Регуляторные/управленческие коэффициенты ликвидности | `UNKNOWN` |
| Полный profit bridge Q2 | `UNKNOWN` |
| Точная декомпозиция NII на repricing / funding cost / mix | `UNKNOWN` |
| Reconciliation ECL 47,7 млрд руб. и implied 41,0 млрд руб. | `UNKNOWN` |
| Точный вклад M&A и органическая динамика г/г | `UNKNOWN` |
| Exact current primary attachment URI 3М/6М2026 | `UNKNOWN` / access-limited |

## 6. Что source universe поддерживает

С наибольшей опорой на завершенные Research Results можно использовать следующие выводы:

- II квартал показал существенное замедление прибыли относительно I квартала и почти flat динамику г/г при сильном росте NII;
- баланс вырос главным образом через cash и клиентское фондирование при сокращении кредитного портфеля;
- 90+ quality metric постепенно ухудшился, при стабильном reserve/gross и снижении reserve/90+ coverage;
- годовые сравнения требуют поправки на изменение периметра группы после приобретения «Европлана»;
- ограниченный доступ к первичным файлам сохраняет существенные KPI и note-level мосты в состоянии `UNKNOWN`.

Source universe **не устанавливает** точные причины изменения NII, прибыли и ликвидности, bank-reported NIM/CIR/CoR, Stage 3, regulatory capital/RWA, официальный liquidity profile или точную органическую динамику после M&A.

## 7. Completion Record

```yaml
scope_boundary:
  bank: "Альфа-Банк"
  reporting_entity: "Группа АО АЛЬФА-БАНК"
  reporting_lens: "консолидированная отчетность по МСФО"
  material_period: "2026-Q2"
  balance_date: "2026-06-30"
  knowledge_cutoff: "2026-09-16"
source_universe:
  - work_id: "IFRS-ALFA-2026-3M-01"
    result_blob: "740b91acb90b06e66bea501b61dd47c381c68cf3"
    terminal_status: "REPORT_EXISTS_ACCESS_LIMITED"
  - work_id: "IFRS-ALFA-2026-6M-01"
    result_blob: "cbd12a019c08dedc5abe20e7f5b6df253f7b4360"
    terminal_status: "completed_bounded_evidence"
reconciliation:
  clean_q2_new_calculation: false
  clean_q2_policy: "inherit only values already established in 6M Research Result; preserve derived/direct-secondary status"
  cross_standard_substitution: false
  external_research_added: false
material_conflicts:
  - "ECL 47.7 direct-secondary vs ~41.0 implied Cbonds gap"
  - "NII before provisions vs Cbonds NII after provisions"
  - "90+ construct vs Stage 3/NPL construct"
material_unknowns:
  - bank_reported_NIM_CIR_CoR
  - Stage2_Stage3_official_coverage
  - regulatory_capital_RWA_liquidity
  - complete_Q2_profit_bridge
  - exact_MA_perimeter_bridge
  - exact_primary_attachments_3M_6M_2026
reliance_envelope: >-
  Suitable as the Alfa-Bank IFRS-only synthesis for Q2 2026 and as a downstream input,
  provided inherited derived values retain their source status, the 3M access limitation remains visible,
  and M&A/perimeter sensitivity is preserved.
stop_basis:
  - both required IFRS Research Works are terminal
  - exact commissioned IFRS source universe is reconciled
  - material conflicts and UNKNOWNs are preserved
  - no cross-standard or external repair evidence was introduced
```
