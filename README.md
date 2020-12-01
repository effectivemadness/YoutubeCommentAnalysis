# Youtube Comment Analysis

crawling all comments from a specific youtube video, and analysis for

- Sentimental Analysis

- wordCloud

- 10 most liked Comments


## introduction

오늘날의 신세대 즉, 밀레니얼 세대(1980년대 초반 ~ 2000년대 초반 출생 세대)[1]와 Z세대(1990년대 중반 ~ 2010년대 중반 출생 세대)[2]에게 Youtube는 정보를 받아들이는 가장 용이한 방법[3]이다.  이면서 이들은 정보 습득에 책, 신문, 편지를 이용하던 기성세대들과도 다르지만, 인터넷으로 검색한 글을 통해 정보를 습득하던 N세대(1970년대 후반 ~ 1980년대 출생 세대)와도 다르다.[4] 이들에게 Youtube는 정보를 습득하는 것 외에 단순히 콘텐츠를 즐기거나[6,7] 자신을 드러낼 수 있는 강력한 플랫폼이다.[5] 최근 5060과 같은 기성세대들의 Youtube 이용 시간도 급증하고 있다. [8]

또한 올해 초 등장한 covid-19의 확산 방지를 위해 거리두기를 지속하면서 접촉하다(tact)의 반대말로 만들어진  ‘언택트(Untact)’라는 뉴노멀(New normal) 트렌드가 생겨났다.[9] 이에 따라 다양한 온라인 플랫폼이 발전하였으며, 특히 영상과 미디어 분야가 두드러진 성장을 보였다. [10]자연스럽게 Youtube를 이용하는 마케팅[11,12], 뉴스 보도, 공연[13] 등 새로운 문화가 형성되었다. 따라서 본 프로젝트는 Youtube의 반응 즉, 댓글을 수집 및 분석함으로서 다양한 분야에서의 활용을 용이하게 하고자 한다.


## workflow

1. crawling comments from specific youtube video with `selenium` from  `python`

2. preprocess data

  - 채팅체 교정 with [`ko-Chat-checker`](https://github.com/seoyoungh/ko-chat-checker)

      - 유투브 댓글은 그 특성상 채팅체로 쓰여져 있는 경우가 많음. 이를 분석 가능한 단어로 교정해주기 위한 모듈 이용

2. sentimental analysis for each comments

3. draw wordCloud for total Comments

4. show 10 most liked Comments



-------------------------------------

### REFERENCE

[1] [밀레니얼 세대, 위키백과](https://ko.wikipedia.org/wiki/%EB%B0%80%EB%A0%88%EB%8B%88%EC%96%BC_%EC%84%B8%EB%8C%80)
[2] [Z세대, 위키백과] (https://ko.wikipedia.org/wiki/Z%EC%84%B8%EB%8C%80)
[3] [이젠 검색도 유투브로 해요](http://m.kisdi.re.kr/mobile/colm/pro_view.m?seq=33517&category=W&selectPage=1)
[4] [디지털 기수, N세대가 온다](http://legacy.h21.hani.co.kr/h21/data/L991011/1p7mab02.html)
[5] [밀레니얼을 말하다- 아싸, 유튜브 세대가 공유를 좋아한다고요?](http://it.chosun.com/site/data/html_dir/2019/01/08/2019010801691.html)
[6] [1020세대, 왜 유튜브에 열광하는가?](http://www.kaa.or.kr/k/mag/2018/05_06/kaa0506_17.pdf)
[7] [밀레니얼 세대는 유튜브에서 논다](https://magazine.hankyung.com/money/article/2019082800172041082)
[8] [레트로 열풍 · 세대간 소통… 유튜브에 빠져드는 5060세대, 세계일보](http://m.segye.com/view/20190712509367)
[9] [IT 트렌드 속성 가이드북- 포스트 코로나, 언택트(Untact)의 시대](https://www.mobiinside.co.kr/2020/06/30/pen-untact/)
[10] [코로나19 확산으로 밀레니얼-Z세대 집콕하며 유튜브 등 SNS 영상과 TV 프로그램 이용 빈도 크게 증가](http://www.asiaa.co.kr/news/articleView.html?idxno=4745)
[11] [유튜브, 밀레니얼 세대를 겨냥한 마케팅 수단](http://www.sobilife.com/news/articleView.html?idxno=27251)
[12] [위기를 기회로! ‘유투브’ 활용한 언택트 마케팅 강세 – 소비자 평가](http://www.iconsumer.or.kr/news/articleView.html?idxno=11326)
[13] [코로나19 시대의 방송 영상 산업, 한국 콘텐츠 진흥원](http://www.kocca.kr/trend/vol22/file/BROADCASTING_TREND_INSIGHT_Vol_22.pdf)
