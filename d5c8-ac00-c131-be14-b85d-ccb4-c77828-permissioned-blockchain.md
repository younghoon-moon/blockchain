# 허가성 블록체인\(Permissioned Blockchain\)

### 0. 개요

비트코인과 이더리움을 비롯한 대부분의 암호화화폐\(cryptocurrency\)는 비허가성\(permission-less\) 블록체인으로 누구나 비트코인 및 이더리움 네트워크에 참가하여 거래내역을 열람 및 검증하거나 화폐발행에 참여할 수 있다. 비허가성 블록체인의 참여자가 되기 위해서 어떠한 허가\(permission\)도 필요하지 않는 것과 반대로 허가성 블록체인은 네트워크에 참여하기 위해서 특정 형태의 허가를 받아야만 한다. 처음 비트코인이 소개된 이후 초기에는 대부분의 블록체인 플랫폼들은 비허가성 플랫폼으로 개발되었으나 최근 들어 금융권과 대기업들을 중심으로 하여 허가성 블록체인에 대한 연구가 활발해지고 있는 추세이다. 금융권에서는 블록체인\(blockchain\)이라는 용어 대신 분산장부기술\(DLT: Distributed Ledger Technology\)라는 용어를 많이 사용하기도 한다. 허가성 블록체인은 비허가성 블록체인과는 완전히 다른 성격을 지니게 되는데 비허가성 블록체인이 현재 가지고 있는 한계점을 극복하는데 중점을 두고 개발되고 있다.

### 1. 개방형\(public\) 비허가성\(permission-less\) 블록체인의 \(현재의\) 한계점

#### 1.1. 확장성\(scalability\)

현재의 대부분의 개방형 블록체인은 초당 처리할 수 있는 거래의 수에 제한이 있는 확장성 문제를 가지고 있다. 예를 들어 현재 비트코인 블록체인은 초당 3~5개, 이더리움은 7~15개 정도의 거래만을 처리할 수 있다. 이는 글로벌 결제업체인 비자\(Visa\)가 초당 약 3,000개 이상의 거래를 처리할 수 있는 것과는 대조적이다. 주식 거래를 처리하는 증권거래소는 초당 수십만건의 거래를 처리하고 사물인터넷\(IoT: Internet of Things\)이 확산되어 수백억개의 스마트 기기들이 기기간 거래\(machine-to-machine payment\)를 하게 되면 이러한 거래를 처리하기에 개방형 블록체인은 한계가 많다.

#### 1.2. 거버넌스\(governance\)

비트코인 및 이더리움과 같은 분산 경제 시스템의 가장 큰 과제 중 하나는 수십조 이상의 시장가치를 갖는 초국가적인 커뮤니티에서 **중요한 정책\(i.e. 프로토콜 변화 혹은 업그레이드\)에 어떠한 방식으로 합의하고 결정할 것인가** 하는 문제이다.

일례로 2017년 8월 1일, 비트코인은 기존의 비트코인\(Bitcoin\)과 비트코인 캐시\(Bitcoin Cash\)라는 두 가지 종류의 비트코인으로 분기\(fork\)되었다. 분기의 가장 큰 이유는 비트코인의 블록크기\(block size\)에 대한 의견대립이었다. 2017년 8월 1일 전까지 비트코인은 블록의 크기가 1MB로 제한되어있었는데 비트코인 코어\(Core\) 개발자들을 중심으로 한 집단은 블록의 크기가 커질수록 네트워크의 대기시간\(latency\)이 길어져 비트코인 네트워크가 중앙화\(centralization\) 된다고 주장하며 블록크기의 증가를 반대했었다. 반면 중국의 채굴자\(miner\)를 중심으로 한 다른 집단은 확장성 문제를 해결하기 위해서는 비트코인의 블록크기를 증가시켜야 한다고 주장하며 비트코인을 분기시켜 비트코인 캐시\(Bitcoin Cash\)를 만들기에 이르렀다.

다른 하나의 대표적인 예는 이더리움\(Ethereum\)과 이더리움 클래식\(Ethereum Classic\)이 있다.

#### 1.3. 데이터 익명성\(data privacy\)

비트코인 거래를 위해서는 [160비트의 비트코인 주소값](https://en.bitcoin.it/wiki/Technical_background_of_version_1_Bitcoin_addresses)을 가명\(pseudonym\)으로 사용한다. 하지만 2009년 비트코인이 처음 동작한 시점부터 모든 거래내역이 누구나 볼 수 있도록 블록체인 상에 기록되어 있어 누군가 나의 주소값을 알고 있다면 나의 비트코인 모든 거래내역을 쉽게 파악할 수 있다. 실제로 이러한 비트코인의 투명성\(transparency\)을 활용하여 전 세계의 법 집행기관\(law enforcement agency\)들은 서로 협력하여 다크 웹\(dark web\) 상의 불법 거래소인 [알파베이\(AlphaBay\)](https://bitcoinmagazine.com/articles/alphabay-shut-down-law-enforcement-admin-commits-suicide-jail/)와 [한사마켓\(Hansa Market\)](https://bitcoinmagazine.com/articles/hansa-market-taken-down-global-law-enforcement-operation/)을 추적하여 불법거래 관련자들을 검거할 수 있었다. 따라서 자신들의 거래내역을 공개하기를 원하지 않는 기업의 경우 비트코인, 이더리움과 같은 개방형 블록체인은 한계가 있을 수 밖에 없다.

### 다양한 허가성 블록체인

R3

Hyperledger

Digital Asset Holdings

EEA\(Enterprise Ethereum Alliance\)

