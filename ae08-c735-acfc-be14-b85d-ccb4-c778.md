# 금융과 블록체인

탈중개인화\(disintermediation\)

### 1. 현재 금융 시스템의 문제점

#### 1.1. **거래 상대방 리스크\(counter-party risk\)**

모든 거래에서는 거래 상대방이 계약의 조건을 이행하지 않을 거래 상대방 리스크\(counter-party risk\)가 존재한다. 특히 아래와 같이 기업간 거래대금의 지급이 지연되는 경우는 비일비재하다.

> 시장 공급사슬 최정점에 있는 영국의 대기업들이 중소기업으로부터 납품을 받고도 기한 내 대금을 지급하지 않고 있어 상대적으로 유동성이 약한 일부 중소기업들이 파산에 이르는 등 산업계 전반에 걸쳐 심각한 피해를 보고 있음. 2012년 12월 마지막 주 집계된 BACS 전자결제 대금지급 지연 규모는 약 364억 파운드\(약 62조 원\)에 달해 사상 최대치를 기록했음. 영국 상공부의 기업거래 규제 대행기관인 ICM에 따르면, 많은 중소기업이 납품 후 평균 180~200일이 지나고도 돈을 받지 못하고 계약상 명시된 대금 지급일보다 평균 41일을 넘기고 있음. [KOTRA](https://news.kotra.or.kr/user/globalBbs/kotranews/3/globalBbsDataView.do?setIdx=242&dataIdx=118726)

이러한 거래 상대방 리스크를 줄이기 위해 비자\(Visa\) 혹은 스위프트\(SWIFT\) 등의 결제 네트워크는 신뢰받는 제3자\(TTP: Trusted Third Party\)로서 차용증서\(IOU\) 관리, 거래 청산\(settlement\), 사기\(fraud\) 방지, 신용분석\(credit analysis\), 신원관리\(identity management\), 리스크 완화\(risk mitigation\) 등을 통해 거래가 안전하게 성사될 수 있도록 한다. 이러한 금융기관들은 거래장부, 신원 및 신용정보 등의 민감한 데이터를 저장하고 처리하기 위해 중앙 데이터베이스\(centralized database\)를 구축 및 관리하는데 중앙화된 시스템은 지나치게 비대하고 비효율적일뿐 아니라 해킹에도 취약하다는 큰 단점이 있다. 이러한 낡은 시스템\(legacy system\)의 유지비용은 고스란히 시스템의 사용자인 상인\(merchant\)들과 소비자\(consumer\)들에게 전가된다.

#### 1.2. **중개인 리스크\(intermediary risk\)**

위에서 보다시피 금융거래 시 거래 상대방 리스크를 줄이기 위해 은행 등의 금융기관들이 중개인\(intermediary\) 역할을 하게 되는데 이 경우 중개인의 시스템이 해킹을 당하거나 자신의 지위를 이용하여 악의적인 행동을 하는 경우가 발생하는 중개인 리스크가 존재한다.

> 한국거래소가 코넥스 기업에게 불합리한 요구 사항을 주문하는 등 갑\(甲\)의 횡포를 저지르고 있는 것으로 나타났다 ... 거래소가 코넥스 기업 주요 주주들에게 보유 지분을 매각하라고 강요하는가 하면 기업 경영진들에게 자체 거래활성화 계획서를 만들어 제출하라고 지시한 것으로 밝혀졌다. [MK증권](http://vip.mk.co.kr/news/2013/1231345.html)

위와 같이 거래소가 자신의 지위를 악용하여 갑질을 하는 사례가 있는 반면 전세사기의 경우처럼 중개인 자체가 조직적으로 사기에 가담하는 경우도 있다.

> 중개무자격자가 중개업등록증을 대여 받아 부동산중개사무소를 차리고, 다른 사람과 공모하여 월세로 여러 채의 주택을 임차한 뒤, 중개업자와 집주인으로 신분을 위장하고 여러 전세 임차인과 중복계약을 체결하여 전세보증금을 가로채는 사례. [부동산114](http://www.r114.com/z/news/research_txt.asp?only=0&m_=6&g_=&bno=200&num=5323&nkind=7&tabmenu=&rgubun=1)

#### 1.3. **청산\(settlement\)**

대부분의 금융거래의 경우 청산에 평균 약 3영업일\(D+3\) 이상이 소요된다.

1.4. **신원관리\(identity management\)**

금융기관들은 사용자의 신원을 확인하기 위해 불필요하게 복잡하고 까다로운 인증절차를 거치게 된다. 우리나라의 공인인증서의 경우 발급하는 절차가 까다로울 뿐 아니라 한 번 발급되면 특정 하드웨어에서만 사용할 수 있어 효율성이 매우 떨어진다.

* **높은 수수료\(high transaction fee\)**: 해외송금의 경우 여러 금융기관을 거쳐 이루어지기 때문에 수수료가 매우 높다. [2012년 기준 이주자\(migrant\)에 의한 국제 송금액은 401억달러](http://blogs.worldbank.org/psd/putting-87-billion-back-pockets-asia-s-migrants)였으며 [평균 송금 수수료는 2017년 6월 기준 7.32%](https://remittanceprices.worldbank.org/sites/default/files/rpw_report_june_2017.pdf)였다. 우리나라에 거주하는 이주 노동자의 경우데도 본국으로 돈을 송금하는데 상당히 많은 수수료를 지불하는데 한국에서 베트남으로 24만원을 송금한다고 하면 [국민은행 혹은 웨스턴유니언\(Western Union\)을 사용하는 경우 각각 21,456원\(8.94%\), 20,688원\(8.62%\)의 높은 수수료를 지불](http://remittanceprices.worldbank.org/en/corridor/South-Korea/Vietnam)해야 한다. 특히 개발도상국들의 낙후된 금융 인프라를 고려하면 실제로 송금받은 돈을 인출하기 위해 멀리 떨어진 은행에 방문해야 하기 때문에 추가적인 시간과 교통비를 고려하면 실질적인 수수료는 더 높을 수 밖에 없다. 가난한 사람들이 더 많은 수수료를 지불해야 하는 악순환이 생긴다. 타지크스탄\(Tajikistan\) 키르기스스탄\(Kyrgyz Republic\), 네팔\(Nepal\)은 본국으로 돈을 송금하는 국제송금\(remittances\)금액이 [GDP의 각각 47%, 31%, 22%를 차지](http://blogs.worldbank.org/psd/putting-87-billion-back-pockets-asia-s-migrants)하는 만큼 자국 노동자들의 국제송금이 경제의 중요한 역할을 담당하기 때문에 송금 수수료 자체가 국가 경제에 매우 큰 영향을 미친다. 특히 우리가 일상생활에서 사용하는 신용카드 결제의 경우에도 중간 수수료가 약 3% 정도로서 결국 소비자들과 상인들이 이 비용을 지불하는 대신 신용카드회사 및 결제 서비스 제공업체들은 두둑한 수수료를 챙긴다. 
* **많은 서류작업\(lots of paperwork\)**: 
* **사생활 보호\(privacy\)**: 자신의 금융 데이터가 중앙서버에 저장되기 때문에 해킹 혹은 검열\(censorship\)에 의해 사생활이 노출된 염려가 있다.
* **해킹 및 사기\(hacking & fraud\)**: 금융기관이 해킹당하는 사례는 많다. 2016년 ["Lazarus"라는 가명을 사용하는 해커](https://en.wikipedia.org/wiki/2015–2016_SWIFT_banking_hack)가 국제 송금망인 [스위프트\(SWIFT: Society for Worldwide Interbank Financial Telecommunication\)망](https://en.wikipedia.org/wiki/Society_for_Worldwide_Interbank_Financial_Telecommunication)을 해킹하여 뉴욕 연방준비은행\(FRB: Federal Reserve Bank\)의 [방글라데시 중앙은행 계좌로부터 약 1억달러를 탈취](http://money.cnn.com/2016/05/26/technology/swift-bank-hack-philippines-lazarus/index.html?iid=EL)하였다. 이와 더불어 2015~2016년에 걸쳐 [베트남](http://money.cnn.com/2016/05/20/news/swift-bank-attack-global-ecuador/index.html?iid=EL), [필리핀](http://money.cnn.com/2016/05/26/technology/swift-bank-hack-philippines-lazarus/index.html?iid=EL), [에콰도르](http://money.cnn.com/2016/05/20/news/swift-bank-attack-global-ecuador/index.html?iid=EL)에서도 SWIFT망 해킹으로 인해 수천만 달러의 자금이 도난 당했다. 각국 중앙은행을 포함하여 전 세계의 대형 은행들이 서로간에 자금을 주고받을 때 사용하는 시스템으로서 "[결제 네트워크의 롤스로이스\(Rollys-Royce\)](https://www.nytimes.com/2016/05/01/business/dealbook/hackers-81-million-sneak-attack-on-world-banking.html)"라 불리 정도로 안전하다고 여겨졌던 스위프트망마저 해킹에 취약하다는 사실이 밝혀지면서 은행과 금융회사들의 시스템에 대한 안정성 문제가 더욱 붉어졌다. 
* **금융의 자유\(financial freedom\)**: 현재 약 25억명의 사람들이 은행계좌를 보유하고 있지 않고 기본적인 은행 서비스에 대한 접근이 불가능한\(unbanked\) 상황.

JPMorgan Chase, Citigroup, and Credit Suisse, all of which are [currently investing](http://www.reuters.com/article/us-axoni-blockchain-idUSKBN149073) in the technology

Santander, a European bank, put the [potential savings at $20 billion a year](http://www.coindesk.com/santander-blockchain-tech-can-save-banks-20-billion-a-year/). Capgemini, a consultancy, estimates that [consumers could save up to $16 billion in banking and insurance fees](https://www.capgemini.com/news/consumers-set-to-save-up-to-sixteen-billion-dollars-on-banking-and-insurance-fees-thanks-to) each year through blockchain-based applications.

The New York–based venture capital firm Union Square Ventures \(USV\) [broadened its investment strategy](https://www.coinbase.com/legal/securities-law-framework.pdf) so that it could buy ICOs directly. Menlo Park venture capital firm Andreessen Horowitz joined USV in [investing in Polychain Capital](http://www.forbes.com/sites/laurashin/2016/12/09/andreessen-horowitz-and-union-square-ventures-invest-10-million-in-new-digital-assets-hedge-fund/#46edeb6a72cd), a hedge fund that only buys tokens. Blockchain Capit\al, one of the industry’s largest investors, [recently announced](http://finteknews.com/blockchain-capital-initial-coin-offering/) that it would be raising money for its new fund by issuing tokens by ICO, a first for the industry. And, of course, companies such as Goldman Sachs, NASDAQ, Inc., and [Intercontinental Exchange](https://en.wikipedia.org/wiki/Intercontinental_Exchange), the American holding company that owns the New York Stock Exchange, which dominate the IPO and listing business, have been [among the largest investors in blockchain ventures](http://money.cnn.com/2015/11/02/technology/bitcoin-1-billion-invested/).

### 2. 블록체인과 금융의 혁신

#### **화폐 \(Currency\)**

각 국가의 중앙은행의 신뢰를 바탕으로 발행되는 법정화폐\(fiat currency\)는 많은 문제점을 가지고 있다. 비트코인은 2008년 금융위기 이후 처음 세상에 알려졌는데 당시는 많은 사람들이 미 정부의 구제금융\(bailout\)을 비판하며 월스트리트 점령운동\(Occupy Wall Street\)을 진행하고 있을 때였다. 월스트리트와 결탁한 권력자들이 대형 투자은행을 구제하기 위해 돈을 찍어내 대형 투자은행 지분의 대부분을 보유하고 있던 상위 1%들은 [조폐이익\(seigniorage\)](https://en.wikipedia.org/wiki/Seigniorage)을 가져가고 99%의 일반 시민들이 이를 [인플레이션세\(inflation tax\)](https://en.wikipedia.org/wiki/Seigniorage#Seigniorage_as_a_tax)의 형식으로 부담하게 됨으로써 하위 99%가 보유하고 있던 부를 상위 1%에게 이전했다는 것이 비판의 골자였다. 비트코인은 [사이퍼 펑크\(cypherpunk\)](https://en.wikipedia.org/wiki/Cypherpunk)를 포함한 [무정부주의자\(anarchist\)](https://ko.wikipedia.org/wiki/아나키즘) 및 [자유주의자\(Libertarian\)](https://ko.wikipedia.org/wiki/자유지상주의)들의 열렬한 지지를 받았는데 그들은 발행량이 한정되어 있고 중앙기관이 통제 및 검열할 수 없는 비트코인에 큰 매력을 느꼈기 때문이다.

이외에도 국가 기반의 화폐 시스템은 많은 문제를 가지고 있다. 예를 들어 베네수엘라는 2017년 예상 약 [700%가 넘는 살인적인 인플레이션](http://premium.mk.co.kr/view.php?no=19409)을 기록하고 있어 자국 화폐에 대한 신뢰기반이 거의 붕괴되었다. 또한 유로존에서는 [그리스 경제위기](https://en.wikipedia.org/wiki/Greek_government-debt_crisis), 이탈리아와 스페인의 재정건정성에 대한 불안감, 브렉시트\(Brexit\) 등의 경제 문제와 시리아 난민의 처리 문제 등의 지정학적 요인에 의해 통화 시스템 자체가 흔들리고 있다. 미국과 중국간의 패권다툼으로 인한 화폐전쟁이 일어날 가능성이 상당하고 중동에서는 ISIS로 인해 국가의 존폐 자체가 흔들리고 있다. 아프리카에서는 정부 자체의 신뢰도가 매우 낮으며 한반도에는 전쟁의 위험이 항상 도사리고 있다. 위와 같은 다양한 문제들의 핵심은 국가라는 중앙기관에 의해 발행되는 화폐들은 해당 **중앙기관이 단일 실패점\(single point of failure\)으로 작용**하게 된다는 것이다.

비트코인을 비롯한 블록체인 기반의 암호화화폐\(cryptocurrency\)는 대부분의 경우 발행량이 한정되어 있으며 화폐에 대한 정책 및 의사결정권한이 분산화된 생태계와 자유시장경제에 의해 결정된다. 비트코인의 등장 이후 수많은 알트코인\(altcoin: alternative coin\)들이 등장했는데 현재까지 수백개의 알트코인들이 시장에서 서로 경쟁하고 있다. 많은 사람들이 이를 오스트리아-헝가리 출신의 경제학자 [프리드리히 하이에크\(Friedrich Hayek\)](https://en.wikipedia.org/wiki/Friedrich_Hayek#Investment_and_choice)가 1976년 그의 저서 “[화폐의 탈국가화\(The Denationalization of Money\)](https://en.wikipedia.org/wiki/The_Denationalization_of_Money)”에서 주장한 민간 발행 화폐의 자유경쟁체계와 비교하기도 한다.

비트코인은 분산화되어 있기 때문에 누구도 비트코인 시스템을 완전히 파괴하기란 불가능하며 비트코인 생태계 또한 개별 국가의 정책에 영향을 적게 받는다. 실제로 2017년 2월 [중국에서 자금세탁방지법\(AML: Anti-Money Laundering\)을 근거로 비트코인 거래소에서의 출금을 금지](https://www.coindesk.com/two-chinas-biggest-exchanges-stop-bitcoin-withdrawals/)한 약 4달의 기간동안 일본이 중국을 제치고 비트코인 거래량 1위가 되었으며 비트코인 가격도 오히려 상승했다.

#### 가치의 이동\(Moving value\)

블록체인은 결제와 해외송금 등 가치의 이동이 필요한 서비스에 사용될 수 있다. 해외송금을 하기 위해서는 웨스턴유니언\(Western Union\)과 같은 해외송급 서비스를 사용해야 하는데 많게는 30~40%나 되는 송금 수수료가 부과된다. 단순 카드결제같은 경우에도 체계가 잘 갖춰진 우리나라의 경우 3%가량이 수수료로 지불되며 기타 국가들은 많게는 10%\(미정\)나 되는 수수료를 부담해야 하는 경우가 많다. 해외에 돈을 송금하기 위해서는 신원확인부터 다수의 서류를 작성하는 등의 지나치게 복잡한 절차를 거쳐야 하며 돈의 액수가 큰 경우에는 더욱 그렇다.

#### **가치의 거래 \(Trading value\)**

현재 대부분의

* 가치의 저장 & 저축\(storing value & savings\)
* 대출 \(lending and borrowing & credit\)

#### 자금유치\(Fund raising\)와 벤처캐피탈\(Venture Capital\)

블록체인은 신생 기업들의 비즈니스 모델 뿐 아니라 자금 확보의 방식까지 완전하게 바꾸어 놓았다. 기존의 스타트업이 시제품\(prototype\)을 만들고 벤처케피탈들을 찾아다니며 사업계획을 피칭하고 여러 라운드의 투자를 유치한 것과는 대조적으로 블록체인 기반의 기업들은 주로 스위스와 같은 암호화 화폐에 대한 규제가 명확한 국가에 재단\(foundation\)을 설립하고 자신의 서비스를 사용할 수 있는 토큰\(token\)을 발행하는 **ICO\(Initial Coin Offering\)**를 진행한다. 기업공개\(IPO: Initial Public Offering\)와는 다르게 복잡한 규제와 까다로운 조건 없이 암호화 화폐를 보유하고 있는 사람이면 누구나 투자할 수 있으며 투자자들은 일정량의 토큰을 투자에 댓가로 받게된다. 이더리움 재단이 백서\(whitepaper\)를 공개하고 2014년 당시 한 달여동안 진행된 크라우드 펀딩을 통해 [210만달러 규모의 자금을 확보](http://insidebitcoins.com/news/ethereum-self-crowdfunded-21-million-in-less-than-a-month-what-is-it-and-why-should-we-care/23838)한 이후 최근의 블록체인 프로젝트인 [테조스\(Tezos\)는 2017년 7월, 42시간만에 2320만달러](https://cointelegraph.com/news/tezos-232-mln-ico-sparks-fresh-fears-for-ethereum-sell-off)를 [뱅코\(Bancor\)는 2017년 6월 12일, 3시간만에 1530만달러의 자금을 유치](https://qz.com/1004892/the-bancor-ico-just-raised-153-million-on-ethereum-in-three-hours/)하는 등 2017년 현재 벤처케피탈보다 많은 금액이 ICO를 통해 블록체인 업계로 유입되고 있다.

현재 ICO 시장이 과열되었다는 의견이 계속해서 제시되고 있고 미국의 증권거래소\(SEC: Securities and Exchange Commission\)도 [보고서](https://www.sec.gov/news/press-release/2017-131)를 통해 ICO를 통해 발행된 토큰이 주식\(securities\)으로 간주될 수 있고 이에 따라 증권거래법에 적용을 받을 수도 있음을 시사했다. 하지만 그럼에도 불구하고 ICO 열기는 멈출줄 모르며 현재에도 수백개의 서비스가 ICO를 준비하고 있다.

#### 신원 및 명성관리\(identity and reputation management\)

보험 및 리스크 관리\(insurance and risk management\)

회계\(accounting\)

감사 및 과세\(audit and tax\)

#### **금융 데이터의 기록 및 보관**

금융 데이터를 안전하게 보관하는 일은 매우 어렵다. 특히 현재의 중앙서버에 기반한 데이터베이스는 효율적으로 거래를 처리할 수 있는 반면 중앙서버가 단일 실패점\(single point of failure\)으로 작용하여 중앙서버가 해킹당하면 시스템 전체가 무너진다.

스마트 컨트랙트를 사용한 각종 금융계약의 자동화

### 3. 블록체인 기반 금융 서비스

#### 화폐\(currency\)

* [**비트코인\(Bitcoin\)**](https://www.bitcoin.com/)**, **[**라이트코인\(Litecoin\)**](https://litecoin.com/): 비트코인과 라이트코인은 분산화된\(decentralized\) P2P 방식으로 중개인없이 발행되고 유통되는 전자화폐로서 인터넷에 접속할 수만 있다면 누구나 쉽게 계좌를 만들고 안전하게 코인을 사고 팔 수 있다. 중앙기관에 의해 발행량이 결정되는 국가 법정화폐\(fiat currency\)와 달리 발행량을 포함한 화폐와 관련된 모든 중요한 의사결정은 분산화된 합의\(consensus\)를 통해서 이루어지기 때문에 어느 한 기관 혹은 개인이 통제할 수 없다. 화폐의 발행 및 거래에 대한 정보는 블록체인이라는 데이터구조에 저장되는데 한 번 블록체인에 기록된 내역은 블록체인에 영구히 저장되어 누구나 열람할 수 있다. 비트코인 및 라이트코인과 같은 암호화화폐\(cryptocurrency\)는 기존의 중앙은행 및 은행과 비자\(Visa\)와 같은 결제업체의 역할을 분산화된 방식으로 구현함으로써 화폐의 발행과 유통의 탈중개인화\(disintermediation\)을 가져온다. 
* **익명성 화폐 -** [**지캐시\(ZCash\)**](https://z.cash/)**, **[**모네로\(Monero\)**](https://getmonero.org/)**, **[**대시\(Dash\)**](https://www.dash.org/): 비트코인의 경우 모든 거래 내역이 비트코인 블록체인에 투명하게\(transparent\) 공개된다. 물론 비트코인 사용자는 [26~35개의 알파벳과 숫자로\(alphanumeric\) 구성된 주소\(address\)](https://en.bitcoin.it/wiki/Address)를 가명\(pseudonym\)으로 사용하긴 하지만 다양한 방식\(e.g. 블록체인 분석\)을 통해 사용자와 주소를 연관\(associate\)시킬 수 있고 한 번 그 연관성이 식별되면 해당 주소를 통한 모든 비트코인 거래 내역을 누구나 볼 수 있어 사생활 보호에 취약하다는 지적이 계속되고 있다. 이러한 문제를 해결하고자 다양한 암호학적\(cryptographic\) 도구를 활용한 새로운 화폐들이 등장했는데 그 대표적인 코인으로는 지캐시\(ZCahs\)와 모네로\(Monero\) 그리고 대시\(Dash\)가 있다. **지캐시\(ZCash\)**는 [영지식증명\(zero-knowledge proof\)](https://en.wikipedia.org/wiki/Zero-knowledge_proof)을 활용한 [zk-SNARKs](https://blog.ethereum.org/2016/12/05/zksnarks-in-a-nutshell/) 프로토콜을 통해 익명성\(confidentiality\)을 보장하는 화폐이며 **모네로\(Monero\)**는 [링 시그니처\(ring signature\)](https://en.wikipedia.org/wiki/Ring_signature), [비밀주소\(stealth address\)](https://getmonero.org/resources/moneropedia/stealthaddress.html), [익명거래\(CT: Confidential Transaction\)](https://elementsproject.org/elements/confidential-transactions/) 등의 다양한 기술을 결합하여 모든 거래를 불투명하게 만드는 화폐이다. 또 다른 디지털 화폐인 **대시\(Dash\)**는 [마스터노드\(masternode\)](https://dashpay.atlassian.net/wiki/spaces/DOC/pages/1867864/What+is+a+masternode)가 존재하여 다양한 거래를 섞어 거래를 보내는 이와 받는 이를 식별할 수 없게 해주는 [프라이빗센드\(PrivateSend\)](https://www.dash.org/news/dashs-privatesend-what-makes-digital-cash-fungible/)의 기능을 수행한다. 익명성은 화폐에 필요한 중요한 특징인 [등가성\(fungibility\)](https://en.wikipedia.org/wiki/Fungibility)과 큰 관련이 있다. 화폐의 등가성이란 **같은 단위의 화폐는 모두 같은 가치를 지녀야 한다**는 것이다. 예를 들어 모든 일만원권 지폐는 같은 가치를 지녀야 한다. 만약 같은 일만원권 지폐가 지폐마다 그 가치가 다르다면 해당 지폐를 받는 사람은 그 지폐의 가치를 신뢰할 수 없게 되어 화폐 시스템의 기본인 신뢰에 금이 가게 되기 때문이다. 비트코인의 경우 거래역사\(transaction history\)가 모두 공개되기 때문에 같은 1BTC라 할지라도 가치가 다를 수 있다. 예를 들어 테러리스트의 자금 유치에 사용되었던 1BTC은 방금 막 발행된 1BTC에 비해 가치가 낮을 수 있는 것이다. 따라서 화폐의 익명성은 각각의 화폐의 거래역사를 추적불가능\(untraceable\)하게 하여 동일 단위의 화폐가 모두 동일한 가치를 지니는 등가성\(fungibility\)을 보장하게 된다. 

ABRA

aeternity

Ripple, Stellar, Dash

Bitshares

Colored Coin

Ethereum

the DAO

#### 자산운용\(Asset Management\)

* **아이코노미\(ICONOMI\): **이더리움 블록체인 기반의 디지털 자산관리 플랫폼으로서 DAA\(Digital Asset Arrays\)라 불리는 디지털 자산의 전략 및 포트폴리오를 운용\(manage\)하는 매니저와 DAA에 투자하는 투자자들을 매칭시켜주는 플랫폼이다. 슬로베니아에 기반을 두고 있으며 2016년 10월 [ICO를 통해 약 1,050만달러의 자금을 유치](https://www.cryptocoinsnews.com/ethereum-based-iconomi-raises-10-5-million-ico/)하였다. 기존의 자산운용사\(asset management\)들을 분산화시키려는 시도이다.
* **멜론포트\(Melonport\)**: 
* 프리즘\(PRISM\)

#### 부동산\(real estate\) 시장

전 세계 거주용 부동산 시장 규모 162조 달러.

20조 달러의 유휴자본\(dead capital\).

개발 도상국은 제대로 된 부동산 등록 시스템 부재

각종 사기\(fraud\)

국가간 부동산 거래의 비효율성과 불편함

the number of transactions in real estate trading is relatively low due to the nature of the sector and the relatively high value of real estate assets

* **프라피\(Propy\): **이더리움 블록체인 기반의 분산화된 부동산 거래 플랫폼 Propy Registry를 통해 전 세계 부동산 자산의 소유권을 추적\(track\)하고 자체 프라피 토큰\(PRO: Propy Token\)을 사용하여 전 세계의 부동산 자산을 등록하고 거래할 수 있도록 해준다.
* 유빗쿼티\(Ubitquity\)
* 팩텀\(Factom\)

#### 헷지펀드\(hedge fund\)

Numerai

Factom

TenX

Exchanges - Bancor, Omisego

Humaniq

