ocenianie takie jak na ISI

1. przykłady tłumaczenia:
 *  korekta tekstu
 *  fonetyzacja
 *  ekstrakcja informacji
 *  przywracanie diakrtyków.
 *  tłumaczenie starych tekstów na nowe

2. Ewaluacja
 *  WER
 *  BLEU - sqrt^4(iloczyn Precision dla unigramów, bigramów, trigramów, tetragramów) * BP

// BP - brevity penalty to kara za zwięzłość


3. precision vs recall:
 *  precision = tp / (tp + fp)
 *  recall  = tp / (tp + fn)
 where:
  t = true
  f = false
  p = positive
  n = negative

4. example:
Expected:   Ala has got a cat
Output:     Alice **has** **cat**

precision = 2/3 = (has cat) / (Alice has cat)
recall = 2/5 = (has cat) / (Ala has got a cat)

