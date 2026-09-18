# Сведение МСФО — Банк ДОМ.РФ, II квартал 2026 года

**Work ID:** `SYN-DOMRF-2026-Q2-IFRS-01`  
**Тип Work:** сведение МСФО одного банка / `THEMATIC_RESEARCH_SYNTHESIS` / MADARAII-12  
**Статус:** `COMPLETE` — терминальный Result текущего цикла  
**Дата сведения:** 2026-09-16  
**Reporting entity:** АО «Банк ДОМ.РФ» и его консолидированная группа  
**Reporting lens:** МСФО  
**Материальный период:** 3М2026, 6М2026 и чистый II квартал 2026 года  
**Исключенный периметр:** ПАО «ДОМ.РФ» как материнская группа  
**Инженерная основа:** `MADARAII/dev@721a199352b5c5282b1478cd6a5eb36a9872fb34`, `FOUNDATION`, `MADARAII-12`, `EXAMPLE-12`  
**Аналитическая основа:** `AM-002.2`, `PROFILE-BANKING`, `METHOD-COMPARE`, `METHOD-DECOMPOSE`, `DEFAULT-BANK-IFRS`

## 1. Контракт сведения и source universe

Цель Work — согласовать два завершенных Research Result Банка ДОМ.РФ, получить чистый II квартал только по совместимым накопленным flow-строкам, сопоставить stock-показатели на 31.03.2026 и 30.06.2026, сохранить ratios как самостоятельные наблюдения и явно удержать конфликты/UNKNOWN.

Source universe закрыт двумя Result одного reporting perimeter:

1. [`Исследования/МСФО/Банк ДОМ.РФ/2026-3М-промежуточная-консолидированная-отчетность/RESULT.md`](../../../../Исследования/МСФО/Банк%20ДОМ.РФ/2026-3М-промежуточная-консолидированная-отчетность/RESULT.md), blob `b3b98b75c0026bd99d0a22d4e9953e7b90428fac`;
2. [`Исследования/МСФО/Банк ДОМ.РФ/2026-6М-промежуточная-консолидированная-отчетность/RESULT.md`](../../../../Исследования/МСФО/Банк%20ДОМ.РФ/2026-6М-промежуточная-консолидированная-отчетность/RESULT.md), blob `967619dd2754dbbea557ca0af2e53a45b46b051f`.

РСБУ, регуляторная отчетность, новости, сектор, макроэкономика, другие банки и новый внешний Research в Work не входят. Первичные и вторичные источники, уже квалифицированные внутри Research Results, используются только через их установленный аналитический смысл и ограничения.

Метод периодизации:

- накопленные совместимые flows: `чистый 2К = 6М2026 − 3М2026`;
- stocks: сравнение `31.03.2026 → 30.06.2026`, без вычитания как потока;
- ratios: отдельные наблюдения соответствующего периода/методики, без арифметического вычитания накопленных коэффициентов;
- несовместимые определения сохраняются раздельно.

## 2. Primary Analytical Result

Во II квартале 2026 года Банк ДОМ.РФ сохранил сильный финансовый результат и перешел от сокращения кредитного stock в I квартале к быстрому балансовому росту. Чистая прибыль чистого II квартала составила **27,352 млрд руб.**, на **5,4%** выше I квартала. Совместимый NII до резервов составил **45,094 млрд руб.**, на **3,8%** выше I квартала. Прибыль до налогообложения выросла квартал к кварталу на **9,6%** до **35,567 млрд руб.**

Рост основных доходов сочетался с повышением вторичного proxy резервной нагрузки: разница между NII до и после резервной строки в Cbonds составила **9,900 млрд руб.** во II квартале против **8,558 млрд руб.** в I квартале. Это `DERIVED_L0` внутри вторичного представления, а не полный ECL charge и не CoR. Полный profit bridge через OPEX, PPOP, ECL и прочие компоненты остается недоступен.

Баланс во II квартале ускорился. Gross loans выросли на **260,1 млрд руб. (+8,0% кв/кв)**, net loans — на **250,7 млрд руб. (+7,9%)**, customer funds — на **323,1 млрд руб. (+9,7%)**. Клиентское фондирование росло быстрее кредитов, поэтому расчетный `net loans / customer funds` снизился с **95,5% до 93,9%**. Это механический balance-sheet факт; вывод о стратегическом изменении фондирования из него отдельно не формируется.

Риск-профиль дает разнонаправленный сигнал. NPL90 снизился с **52,0 до 42,1 млрд руб. (-19,0% кв/кв)**, а доля NPL90 в gross loans — с **1,60% до 1,20%**. Одновременно резерв вырос с **84,1 до 93,5 млрд руб. (+11,2%)**, а reserve/gross loans — с **2,59% до 2,66%**. Поэтому снижение узкой просрочки во II квартале нельзя трактовать как общее снижение кредитного риска. Накопленный CoR 6М2026 равен **1,1%**, но CoR 3М2026 в сопоставимой reported-методике отсутствует, поэтому чистый CoR II квартала остается `UNKNOWN`.

Бизнес-модель сохраняет project-finance специализацию, однако между отчетными точками присутствует жесткая граница определения: **1,9 трлн руб. на 31.03.2026** относится к выбранному портфелю проектного финансирования жилья, тогда как headline **свыше 8 трлн руб. на 01.07.2026** относится к контуру лимитов/обязательств. Эти величины не образуют временной ряд. Выбранный PF book на 30.06.2026 остается `UNKNOWN`.

## 3. Чистый II квартал: совместимые накопленные flows

| Показатель | 3М2026 | 6М2026 | Чистый 2К2026 | 2К к 1К | Статус |
|---|---:|---:|---:|---:|---|
| Чистая прибыль | 25,946 | 53,298 | **27,352 млрд руб.** | **+5,4%** | `DERIVED_L0`, совместимые cumulative lines |
| Прибыль до налогообложения | 32,461 | 68,028 | **35,567 млрд руб.** | **+9,6%** | `DERIVED_L0-secondary` |
| NII до резервов | 43,434 | 88,528 | **45,094 млрд руб.** | **+3,8%** | `DERIVED_L0`, одинаковая line definition Cbonds; уровни согласуются с reported 43,4 / 88,5 |
| NII после резервной строки | 34,876 | 70,070 | **35,194 млрд руб.** | **+0,9%** | `DERIVED_L0-secondary`; отдельный construct |
| Разница NII до/после резервной строки | 8,558 | 18,458 | **9,900 млрд руб.** | **+15,7%** | `DERIVED_L0-secondary`; proxy, не полный ECL |
| Чистый комиссионный доход | около 3,7 | 9,1 | **около 5,4 млрд руб.** | — | `DERIVED_L0-approx`; исходные reported значения округлены |

Все значения в таблице — млрд руб. Чистый квартал рассчитывается только там, где Research Results сохраняют совместимую накопленную строку. Для комиссионного результата точность ограничена округлением исходных reported значений.

### Интерпретация flow-bridge

- Чистая прибыль и PBT во II квартале были выше I квартала, то есть сильный результат 6М сформирован двумя сопоставимыми по масштабу кварталами, а не одним разовым I кварталом.
- NII до резервов вырос на 1,660 млрд руб. кв/кв; одновременно вторичный резервный proxy вырос на 1,342 млрд руб. Полный вывод о драйверах прибыли требует OPEX/PPOP и точного ECL, которые остаются `UNKNOWN`.
- Чистый комиссионный доход во II квартале ориентировочно превышал I квартал, однако округление исходных значений ограничивает точный q/q-темп.

## 4. Баланс: stocks 31.03 → 30.06

| Показатель | 31.03.2026 | 30.06.2026 | Изменение за 2К | q/q | Статус |
|---|---:|---:|---:|---:|---|
| Активы | 4 543,161 | 4 756,676 | **+213,515 млрд руб.** | **+4,7%** | `OBSERVED_L0-secondary` |
| Gross loans | 3 251,774 | 3 511,912 | **+260,138 млрд руб.** | **+8,0%** | `OBSERVED_L0-secondary` |
| Net loans | 3 167,706 | 3 418,422 | **+250,716 млрд руб.** | **+7,9%** | `OBSERVED_L0-secondary` |
| Customer funds | 3 318,334 | 3 641,457 | **+323,123 млрд руб.** | **+9,7%** | `OBSERVED_L0-secondary` |
| Обязательства | 4 085,330 | 4 277,520 | **+192,190 млрд руб.** | **+4,7%** | `OBSERVED_L0-secondary` |
| Equity, расчетно | 457,831 | 479,156 | **+21,325 млрд руб.** | **+4,7%** | `DERIVED_L0`, assets − liabilities |
| Денежные средства и эквиваленты | 464,190 | около 270,6 | **−193,6 млрд руб.** | **−41,7%** | `OBSERVED_L0-secondary`; одна строка cash не определяет liquidity buffer |

### Траектория первого полугодия

Gross loans сначала снизились с 3 340,742 млрд руб. на конец 2025 года до 3 251,774 млрд руб. на 31.03.2026 (**−2,7% YTD**), затем выросли до 3 511,912 млрд руб. во II квартале (**+8,0% q/q**), что дало **+5,1% за 6М**. Customer funds в I квартале выросли лишь на **0,7%**, а во II — на **9,7%**, сформировав **+10,5% за 6М**.

Таким образом, II квартал изменил внутригодовую траекторию: кредитный портфель вернулся к росту, а клиентское фондирование ускорилось еще сильнее.

## 5. Фондирование и reporting-definition conflict

| Показатель | 31.03.2026 | 30.06.2026 | Изменение |
|---|---:|---:|---:|
| Net loans / customer funds | 95,5% | 93,9% | **−1,6 п.п.** |
| Gross loans / customer funds | 98,0% | 96,4% | **−1,6 п.п.** |

Главный пригодный квартальный funding-series — точная total-line customer funds из одного вторичного IFRS extraction. Она показывает рост на 323,1 млрд руб. за квартал.

При этом сегментное розничное фондирование между двумя Research Results **не сопоставимо без дополнительного bridge**:

- 3М Result: официальный уровень вкладов и счетов физлиц около **0,7 трлн руб.**, отдельное раскрытие — **704 млрд руб.**, рост +9% / +11% YTD в двух сообщениях;
- 6М Result: официальный уровень средств физлиц около **1,7 трлн руб.**, +10% YTD; средства юрлиц — около **2,0 трлн руб.**, +11% YTD.

Уровни 0,7 и 1,7 трлн руб. при близких YTD-темпах не могут образовывать один непрерывный construct без изменения состава/классификации или иной reporting-definition. Причина внутри закрытого source universe не установлена. Поэтому квартальный прирост физлиц из этих двух значений **не рассчитывается**, а конфликт сохраняется как `UNKNOWN / DEFINITION BREAK`.

Кроме того, округленные 1,7 + 2,0 трлн руб. превышают точную total-line 3,641 трлн руб.; эти компоненты используются только как ориентир структуры и не складываются механически.

## 6. Кредитный риск: stock и flow разводятся

| Показатель | 31.03.2026 | 30.06.2026 | Изменение | Статус |
|---|---:|---:|---:|---|
| Резерв по кредитам | 84,068 | 93,490 | **+9,422 млрд руб. / +11,2%** | `OBSERVED_L0-secondary` |
| Reserve / gross loans | 2,59% | 2,66% | **+0,08 п.п.** | `DERIVED_L0` |
| NPL90 | 51,981 | 42,128 | **−9,853 млрд руб. / −19,0%** | `OBSERVED_L0-secondary` |
| NPL90 / gross loans | 1,60% | 1,20% | **−0,40 п.п.** | `DERIVED_L0` |
| Reserve / NPL90 | 161,7% | 221,9% | **+60,2 п.п.** | `DERIVED_L0`, широкий proxy; не Stage 3 coverage |

После резкого роста NPL90 в I квартале показатель частично нормализовался во II. При этом на 30.06.2026 NPL90 **42,128 млрд руб.** все еще выше уровня конца 2025 года **37,376 млрд руб.**, а доля **1,20%** немного выше **1,12%** на 31.12.2025. Поэтому q/q-улучшение не означает возврат risk stock к уровню начала года.

Резерв, напротив, рос в обоих кварталах и к 30.06.2026 достиг 93,490 млрд руб. Рост reserve stock при снижении NPL90 может отражать иные risk buckets, migration, model overlays или иной состав ожидаемых потерь, однако внутри source universe такая причина не идентифицирована. Любая конкретная причинная атрибуция остается `UNKNOWN`.

Накопленный reported CoR 6М2026 — **1,1%** против **0,9% за 2025 год**. Поскольку сопоставимый CoR 3М2026 отсутствует, чистый II квартал по CoR не вычисляется.

## 7. Маржа, эффективность, рентабельность и капитал

Ratios не рассматриваются как additive flows:

- NIM за 3М2026 — **4,4% reported**; NIM за 6М2026 в доступном Result — `UNKNOWN`. Q2 NIM — `UNKNOWN`.
- ROE за 3М2026 — **23,8% reported** по методике Банка. Значение **23,32%** на 30.06.2026 — `secondary-derived` Cbonds с иной/неподтвержденной методикой. Прямой q/q bridge ROE не строится.
- CIR, OPEX и PPOP в сопоставимом IFRS-периметре остаются `UNKNOWN`, поэтому полная оценка операционной эффективности II квартала отсутствует.
- Расчетный IFRS equity proxy вырос с 457,8 до 479,2 млрд руб. во II квартале. Это бухгалтерский residual `assets − liabilities`, а не регуляторный капитал.
- Capital adequacy, RWA, RWA density и полный liquidity buffer на 30.06.2026 остаются `UNKNOWN`.

Снижение cash с 464,2 до около 270,6 млрд руб. не используется как самостоятельный вывод об ухудшении ликвидности: полный liquidity contour отсутствует.

## 8. Project finance и розничная нормализация

### 8.1. Project finance

На 31.03.2026 Research Result фиксирует **1,9 трлн руб. выбранного портфеля проектного финансирования жилья**. На 01.07.2026 6М Result фиксирует **свыше 8 трлн руб.** в контуре проектного финансирования, но квалифицирует эту величину как лимиты/обязательства, а не drawn balance.

Следовательно:

- `1,9 трлн → >8 трлн` не является ростом портфеля;
- q/q growth drawn PF book — `UNKNOWN`;
- `drawn / committed`, escrow balance/coverage, PF CoR и Stage 2/3 проектного портфеля — `UNKNOWN`;
- для межбанковского анализа committed limits и балансовые corporate loans должны сохраняться раздельно.

### 8.2. Розничный кредитный портфель

6М Result сообщает сокращение розничного credit stock на **12% YTD**, одновременно фиксируя секьюритизацию собственных кредитов на **130,7 млрд руб.** и ипотечные выдачи **73 млрд руб. за 6М**, +55% г/г.

Секьюритизация является материальным фактором балансовой динамики. Поэтому снижение retail stock само по себе не доказывает снижение кредитной активности. Точный нормализованный retail bridge в закрытом source universe отсутствует и сохраняется как `UNKNOWN`.

## 9. Reconciliation conflicts и ограничения

1. **Retail funding 0,7 трлн vs 1,7 трлн.** Два официальных уровня из Research Results не образуют сопоставимый ряд при заявленных близких YTD-темпах. Причина `UNKNOWN`; квартальный retail-funding bridge запрещен.
2. **PF 1,9 трлн vs >8 трлн.** Разные constructs: drawn book против лимитов/обязательств. Сравнение как временного ряда запрещено.
3. **NII y/y growth.** Для 3М официальный рост +68% расходится с механическим +73,6% по Cbonds; для 6М +52% расходится с +56,5%. Уровни текущего периода пригодны для clean-Q2 bridge, причины comparator conflicts остаются `UNKNOWN`.
4. **NII до/после резервов.** 43,434/88,528 и 34,876/70,070 — разные строки. Они сохраняются отдельно.
5. **ROE.** 3М reported 23,8% и 6М Cbonds 23,32% имеют разные/неподтвержденные denominator и annualization; прямое сравнение ограничено.
6. **NPL90 ≠ Stage 3.** Узкая просрочка 90+ не заменяет Stage 3/POCI. Stage-based quality и coverage остаются `UNKNOWN`.
7. **Secondary extraction.** Значительная часть balance/risk stock получена через Cbonds в исходных Research Results из-за ограниченного доступа к primary PDF. Синтез не повышает их evidence status.
8. **Parent perimeter.** Показатели ПАО «ДОМ.РФ» исключены. Значения parent group не используются для заполнения банковских пробелов.

## 10. Material UNKNOWNs

В итоговом IFRS-контуре Банка ДОМ.РФ за II квартал остаются существенными:

- чистый Q2 CoR и точный Q2/full-period ECL charge;
- Stage 1/2/3/POCI, Stage 2/3 shares и reported coverage;
- Q2/6М NIM;
- OPEX, PPOP, CIR и cost of funding в сопоставимом IFRS-периметре;
- exact corporate/retail loan bridge между 31.03 и 30.06;
- сопоставимый retail/corporate/escrow funding mix и причина retail-funding definition break;
- drawn PF book на 30.06, committed utilization, escrow balances/coverage и PF risk metrics;
- capital adequacy, RWA, RWA density и полноценный liquidity buffer;
- причины исторических comparator conflicts по NII.

Эти UNKNOWN ограничивают детализацию, но не меняют установленные выводы по чистой прибыли, NII, общему балансовому росту, total customer funds и наблюдаемой динамике NPL90/reserve stock.

## 11. Analytical Basis и source accounting

| Source Result | Роль в синтезе | Что передано | Ограничения сохранены |
|---|---|---|---|
| 3М2026 Result | Q1 cumulative flow baseline + stocks 31.03 | прибыль, PBT, NII, secondary reserve bridge, комиссии, assets/loans/funds, reserve, NPL90, Q1 NIM, PF drawn snapshot | primary PDF access gap; Stage/ECL/CoR/efficiency/capital UNKNOWN; funding-definition conflict |
| 6М2026 Result | H1 cumulative flows + stocks 30.06 | прибыль, PBT, NII, комиссии, CoR 6М, assets/loans/funds, reserve, NPL90, секьюритизация, PF limits contour | primary PDF access gap; Stage/NIM/efficiency/capital/liquidity UNKNOWN; PF drawn 30.06 UNKNOWN |

Синтез выполнил только арифметические derivations и reconciliation внутри этого universe. Новый внешний источник, новый Research и другой reporting lens не вводились.

## 12. Completion Record

```yaml
scope_boundary: "АО «Банк ДОМ.РФ» и его консолидированная группа, IFRS-only synthesis 3М/6М2026 и чистый II квартал"
source_universe:
  - "IFRS-DOMRF-2026-3M-01 RESULT.md @ b3b98b75c0026bd99d0a22d4e9953e7b90428fac"
  - "IFRS-DOMRF-2026-6M-01 RESULT.md @ 967619dd2754dbbea557ca0af2e53a45b46b051f"
coverage:
  - concern: clean_q2_compatible_flows
    state: analyzed
  - concern: balance_credit_and_total_funding_stocks
    state: analyzed
  - concern: credit_risk_stock_vs_flow
    state: analyzed_with_limits
  - concern: profitability_and_margin
    state: partially_analyzed
  - concern: project_finance_construct_bridge
    state: analyzed_with_material_unknowns
  - concern: retail_securitization_normalization
    state: partially_analyzed
  - concern: efficiency_capital_liquidity
    state: unresolved
material_unknowns:
  - "Q2 CoR / exact ECL and Stage migration"
  - "6М/Q2 NIM; OPEX/PPOP/CIR/cost of funding"
  - "30.06 drawn PF book, escrow and PF quality"
  - "retail funding definition break 0.7tn vs 1.7tn"
  - "capital adequacy/RWA and full liquidity contour"
residual_risks:
  - "secondary IFRS extraction may differ from primary PDF vintage/classification"
  - "method-sensitive ratios cannot be peer-ranked without passport alignment"
  - "rounded official segment values cannot replace exact total lines"
stop_basis:
  - "both required IFRS Research Results are terminal and use the same reporting perimeter"
  - "all compatible cumulative flow lines needed for clean-Q2 bridge are reconciled"
  - "material stock, ratio, definition conflicts and UNKNOWNs have explicit dispositions"
  - "further closure would require new or reopened Research outside this Commission"
reliance_envelope: "bank-level IFRS period synthesis and downstream cross-bank work; no substitution with RAS, parent-group or news data"
terminal_status: "COMPLETE for ordinary current cycle; reopening requires a separate direct Commission"
```

## 13. Итог для последующего межбанковского контура

Для сопоставления Банка ДОМ.РФ с другими банками надежно передаются: **чистая прибыль II квартала 27,352 млрд руб.; NII II квартала 45,094 млрд руб.; gross loans 3,512 трлн руб.; net loans 3,418 трлн руб.; customer funds 3,641 трлн руб.; q/q рост gross/net loans 8,0%/7,9%; q/q рост customer funds 9,7%; NPL90 1,20%; reserve/gross loans 2,66%.**

Отдельно должны сохраняться ограничения: CoR II квартала, NIM II квартала, Stage quality, CIR, capital/RWA, liquidity и drawn PF book на 30.06 остаются `UNKNOWN`; project-finance limits свыше 8 трлн руб. не являются балансовым кредитным портфелем; retail funding между 3М и 6М имеет unresolved definition break.
