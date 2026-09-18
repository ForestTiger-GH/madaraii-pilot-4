> **HISTORICAL / SUPERSEDED BY CARRIER 013.** Текущими являются `КАРТА-ТЕМ-DEEP-REOPEN-2026-2К.md` и `МЕЖБАНКОВСКОЕ-DEEP-REOPEN-2026-2К/RESULT.md` соответственно роли. Этот файл сохранен только как history/challenge и не является current owner.

# Enriched banking core — II квартал 2026

**Work:** MADARAII-10, first-pass challenge/enrichment.  
**Backbone:** `МЕЖБАНКОВСКОЕ-ПОВТОР-2026-2К.md`.  
**Challenge universe:** 34 first-pass syntheses; исходные status ceilings сохранены.

## Result

First-pass слой materially не опроверг repeat-only core-10. Совпадающие направления классифицированы как CONFIRM либо DUPLICATE_UPSTREAM; дополнительные детали — UNIQUE_ENRICHMENT/CONTEXT; старые элементы, замененные repeat-перечтением, — SUPERSEDED; несводимые расхождения сохранены как CONFLICT/CONTEXT. Material conflict, требующий reopen repeat core, не установлен.

Secondary comparators расширяют картину:
- Совкомбанк: Q2 улучшение margin/profit и corporate growth; M&A меняет perimeter, organic like-for-like ограничен.
- МТС Банк: first-pass IFRS показывает улучшение Q2 прибыльности/NIM и снижение текущей reserve burden.
- Райффайзенбанк RAS: assets +2,3%, loans +1,7%, Q2 profit около flat; 6M YoY слабее; standalone IFRS недостаточен.
- НОВИКОМ RAS: assets около +16%, Q2 profit -50,6% q/q при примерно стабильном NII; IFRS terminal NOT_FOUND_UNDER_BOUNDED_SEARCH.
- Яндекс Банк RAS: assets +21%, retail loans +32,5%, customer funding +15,4%, capital ratios укрепились; standalone IFRS bounded search отрицательный.
- ВБ Банк RAS: assets +24,4%, funds +50,9%, loans +6,9%, fee-heavy disclosed income; RWA +20,6% при capital +3,7%; IFRS insufficient.
- Т-Технологии IFRS и ТБанк RAS — разные perimeter. Group Q2 NII +31,8% y/y, NIM 11,6%, CoR 4,7%, profit 39,5 млрд руб. с -21,8 млрд investment revaluation; standalone RAS profit 37,9 млрд руб., -24,9% q/q при улучшении процентного spread и росте OPEX.

## Enriched model

1. Улучшение ЧПД во многих банках связано с более быстрым снижением процентных расходов; macro-causal attribution пока не установлена.
2. Быстрый balance growth у ПСБ, Озона, Яндекса, ВБ и НОВИКОМа часто сопровождается ускорением RWA, OPEX или reserve burden.
3. Platform banks имеют высокие темпы funding/fees и малую базу; их disclosure/perimeter требуют отдельного comparison universe.
4. Quality of earnings materially зависит от one-offs/perimeter: M&A Совкомбанка, investment revaluation Т-Технологий, hidden residual ПСБ, dividend timing Сбера, securitization/FV effects ДОМ.РФ.
5. Missing disclosure НОВИКОМа/Яндекса/ВБ не трактуется как слабый риск и не заполняется средним.

**UNKNOWN:** единые NIM/CIR/CoR/ROE extended-17; platform standalone IFRS comparability; common capital headroom; standardized RAS credit-quality stocks; market shares без common denominator; causal repricing.

Repeat-only baseline остается отдельным Result. Следующий route — Theme Mapping полного корпуса.


## T1 thematic Result — Макрорежим и процентная экономика

Q2 сочетал снижение ключевой ставки 15,0→14,25%, жесткие финансовые условия и ускорение кредита. Во многих банках ЧПД вырос через более быстрое снижение процентных расходов. Это MECHANICAL_L1; общий repricing mechanism поддержан sector evidence, но bank-specific CAUSAL_L3 остается UNKNOWN без price/volume/mix.


## T2 thematic Result — Кредитование, фондирование, ликвидность и капитал

Sector corporate claims +3,7% q/q и retail lending ускорились. Bank trajectories различались: Сбер/ВТБ/МКБ показали более плотный loan-to-funds профиль; ПСБ, ДОМ.РФ, ОТП, Озон и platform banks наращивали клиентские средства. MECHANICAL_L1: рост loans/RWA быстрее capital сжимает capital ratios при росте абсолютного капитала; это видно у ДОМ.РФ, Озона и ВБ. Liquidity ratios methodology-specific. Debt programs не равны funding inflow. UNKNOWN: common capital headroom, comparable LCR/NSFR, standardized L/F.
