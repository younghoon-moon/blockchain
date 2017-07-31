# 비트코인\(Bitcoin\)과 블록체인\(blockchain\) {#d}

2008년 11월 1일 사토시 나카모토\(Satoshi Nakamoto\)라는 가명의 인물이 [암호학 메일링 리스트](http://satoshi.nakamotoinstitute.org/emails/cryptography/1/#selection-14.11-51.41)를 통해[ "비트코인: P2P 전자화폐 시스템 \(Bitcoin: A Peer-to-Peer Electronic Cash System\)"](http://www.bitcoin.org/bitcoin.pdf)이라는 제목의 백서 공개. 이후 메일링 리스트에 포함되어 있던 다른 사람들과 [지속적으로 의견을 교류](http://satoshi.nakamotoinstitute.org/emails/cryptography/)하고 이 2009년 1월 9일 [비트코인 버전 0.1을 출시](http://satoshi.nakamotoinstitute.org/emails/cryptography/16/#selection-19.39-23.43)하였음.

### 1. 비트코인의 구조

비트코인은 크게 다음의 네 가지 요소로 구성되어 있음.

* **블록체인\(blockchain\)** 구조의 데이터베이스
* 데이터베이스에 누가 어떻게 데이터를 추가시킬 것인지를 결정하는 **합의 메커니즘\(consensus mechanism\)**
* 비트코인\(Bitcoin\)이라 불리는 **토큰\(token\)**
* 비트코인 클라이언트\(client\) 소프트웨어를 운영하는 노드\(node\)로 구성된 **P2P\(peer-to-peer\) 네트워크**

#### 1.1. 블록체인\(blockchain\)이란?

블록체인은 블록들이 체인 구조로 연결되어 있는 데이터베이스이다. 비트코인 블록체인에는 매 10분마다 새로운 블록이 추가되며 각 블록은 비트코인으로 이루어진 거래내역 데이터를 담고 있다. 블록체인은 이른바 전 세계에서 비트코인으로 이루어지는 거래의 내역이 모두 기록되는 장부\(ledger\)인 것이다. 각 블록은 이전 블록의 아이디값을 포함하고 있어 블록체인의 중간에 있는 블록을 수정하기 위해서는 해당 블록 이후에 생성된 모든 블록을 수정해야 한다.

#### 1.2. 합의 메커니즘\(consensus mechanism\)이란?

블록체인은 비허가성\(permission-less\) 분산화\(decentralized\) 장부로서 기존의 단일 중앙 데이터베이스에서는 발생하지 않는 문제들이 중요하게 대두된다. 기존의 단일 중앙 데이터베이스의 경우에는 은행과 같은 신뢰받는 제 3자\(TTP: Trusted Third Party\)가 데이터베이스에 대한 독점적 수정권한을 바탕으로 거래내역을 기록하고 수정하는 반면 비트코인은 이러한 중개인\(intermediary\) 없이 서로 신뢰하지 않는 다수의 참가자들이 모두 동의할 수 있는 방식으로 거래내역을 기록해야 하는 과제를 앉고 있다. 따라서 거래내역의 정당성\(validity\)에 대해 누구나 객관적으로 검증\(verify\)하고 이를 통해 단일의 거래내역에 합의\(consensus\) 할 수 있는 방식과 절차가 필요한데 이를 합의 메커니즘\(consensus mechanism\)이라 한다.



#### 1.3. \(토큰으로서의\) 비트코인이란?

#### 1.4. 비트코인 네트워크란?







### 2. 비트코인의 특성

비트코인은 다음과 같은 특성을 갖는다.

* 분산화\(Decentralization\)
* 투명성\(Transparency\)
* 익명성\(Anonymity\)
* 비허가성\(Permission-less-ness\)
* 비가역성\(Immutability\)
* 검열 저항성\(Censorship Resistance\)



















