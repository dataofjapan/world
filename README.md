# Data of Japan
## World

* countryCodesFull.tsv

ISO 3166で規定されている国の名称や国コード一覧。
datahub( http://datahub.io/dataset/iso-3166-1-alpha-2-country-codes )上のデータを取得（取得日は2014年7月15日）し、以下の改変を行った。

削除：
ISO 4217 Currency Code, ISO 4217 Currency Name, ITU-T Telephone Code, IANA Country Code TLD

名称変更：
ISO 3166-1 2 Letter Code -> 2LetterCode
ISO 3166-1 3 Letter Code -> 3LetterCode
ISO 3166-1 Number -> NumberCode

* countryCodes.tsv

countryCodesFull.tsvを元に、実案件での使い勝手を考慮してさらにいくつか情報をトリミングした。

削除：
FormalName, Type, SubType, Sovereignty, Independent StateのProto Independent Stateのどちらにも当てはまらないTypeの国

