| # | 資料・機関 | 対象 | URL | k=3に関する記載（原文） | 和訳 | 証拠の強さ | 何の根拠になるか |
|---|---|---|---|---|---|---|---|
| **1** | **NHS England**<br>*Anonymisation Standard for Publishing Health and Social Care Data Specification*<br>2013 | 医療・社会福祉データ | https://digital.nhs.uk/binaries/content/assets/website-assets/isce/isb1523/1523202010spec.pdf | **“Weak” k-anonymity is where:<br>• K = 3**<br><br>また、k-anonymityの定義として、<br>**“the information for each person contained in the data set cannot be distinguished from at least k-1 individuals”** | **「弱いk-匿名性」とはK=3とするもの。**<br><br>また、各人について、その人の情報が**少なくともk−1人の他の個人の情報と区別できない**場合、k-匿名性を満たすとする。<br><br>したがってk=3なら、**本人＋他の2人**となる。 | **★★★★★** | **医療データについて公的機関がk=3を明示した根拠。**<br>さらに「k−1人」という定義があるため、**「本人を除いて2人」**という解釈の直接的な根拠になる。 |
| **2** | **IHSN**<br>*Introduction to Statistical Disclosure Control (SDC)*<br>IHSN Working Paper No.007<br>2014 | 統計ミクロデータ<br>（標本調査・国勢調査等） | https://ihsn.org/sites/default/files/resources/ihsn-working-paper-007-Oct27.pdf | **“A typical practice is to set k = 3”**<br><br>続いて、<br>**“the same pattern of key variables is possessed by at least three records in the sample.”** | **「典型的な実務ではk=3とする。」**<br><br>これにより、同じkey variablesのパターンを**少なくとも3レコード**が共有することになる。 | **★★★★☆** | **k=3が統計ミクロデータ匿名化における「典型的な実務値」であることの根拠。**<br>ただし、**なぜ3なのかという理由は記載されていない。** |
| **3** | **カナダ／El Emam et al.**<br>*De-identifying a public use microdata file from the Canadian national discharge abstract database*<br>2011 | カナダ全国入院患者データ<br>（DAD） | https://pmc.ncbi.nlm.nih.gov/articles/PMC3179438/ | **“We will assume that we are aiming for k = 3”**<br><br>また、再識別リスクについて、<br>**“This is measured by 1/k within the context of the k-anonymity criterion.”** | 医療データの匿名化例において、**k=3を目標とする**と設定。<br><br>また、k-匿名性の文脈では、正しく再識別される確率を**1/kで測定する**としている。<br><br>したがってk=3なら、単純化すると**1/3（約33%）**という対応になる。 | **★★★★☆** | **医療データでk=3を実際に適用した根拠。**<br>さらに、**kと再識別確率1/kを結び付けている**点が重要。 |
| **4** | **Pacific Community (SPC)**<br>*Methodological review for anonymising census and survey microdata in the context of Small Island Developing States*<br>2024 | Census・Surveyのミクロデータ | https://www.spc.int/digitallibrary/get/kztoa | **“typical practice is to set k = 3 but it is difficult to ascertain how this was established.”** | **「典型的な実務ではk=3とされているが、それがどのように確立されたのかを確認することは困難である。」** | **★★★★★（k=3の由来調査として）** | **k=3が慣行として存在する一方、「なぜ3なのか」という成立根拠が明確でないことを示す根拠。** |



| 論点 | エビデンス |
|---|---|
| **k=3という基準は存在する** | NHS、IHSN、Canada、SPC |
| **統計分野でk=3は典型的な実務値** | IHSN、SPC |
| **医療データでもk=3が使われている** | NHS、Canada |
| **k=3は「本人＋2人」という意味になる** | NHSの「k−1 individuals」 |
| **k=3と再識別確率1/3を結び付ける考え方がある** | Canada / El Emam |
| **「なぜ3なのか」の明確な歴史的根拠** | **現時点では確認できない** |
| **k=3は数学的に導出された必然値ではない** | SPCの記述から少なくともそのように扱われている |
