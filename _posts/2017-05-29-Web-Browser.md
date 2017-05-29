---
layout: post
title: All about Pesitting Web UI!
---

블록체인 기반 펫시팅 서비스 - 웹 어플리케이션 구현

펫시팅 서비스를 하기 위해선 웹 어플리케이션 구현이 필요합니다.
우선 웹에 기본적으로 필요한 회원정보, 펫시터정보, 자산(집, 펫)정보를 등록할 수 있는 환경이 필요합니다.

회원정보와 펫을 담고 있는 저장 매체는 데이터베이스를 이용하고 펫시터와 집 정보를 저장하는 곳은 블록체인입니다.

그렇다면 먼저 회원정보에 대해서 알아보도록 하겠습니다.

![_config.yml]({{ yozzung.github.io }}/images/log-in.png)
![_config.yml]({{ yozzung.github.io }}/images/sign-up.png)

위 사진을 보면 회원 정보의 기본이 되는 이메일과 비밀번호를 받게 됩니다. 회원등록 이외에 모든 정보는
이메일을 기분으로 이루어지기 때문입니다.
그 뒤 로그인을 한 사용자는 펫시터 검색, 집 등록, 펫시터 등록, 펫 등록이라는 기능을 추가로 이용할 수 있게 됩니다.

![_config.yml]({{ yozzung.github.io }}/images/search_home.png)
![_config.yml]({{ yozzung.github.io }}/images/search_result.png)

사용자가 검색한 바탕으로 블록체인에 저장되어 있던 모든 펫시터에 대한 리스트를 받아 보여주게 됩니다.

그렇다면 이런 펫시터들의 정보는 어떻게 저장하고 있는지 알아볼까요?

먼저 펫시터가 있어야 합니다. 펫시터가 있기 위해선 어떻게 되야할까요?
펫시터가 되길 희망하는 사람은 집을 등록해야합니다.
그래야 사용자가 신뢰를 가지고 마음 편히 자신의 펫을 맡길 수 있기 때문입니다.

![_config.yml]({{ yozzung.github.io }}/images/enroll_house.png)
![_config.yml]({{ yozzung.github.io }}/images/house_list.png)

그럼 이용하는 사람은 이런 의문이 생길 수 있습니다. 해당 펫시터가 거짓으로 집을 등록한 것이면 어쩌지?

하지만 그런 의문점을 해결하기 위해 블록체인을 기반으로 한다고 이야기하면 앞의 블록체인에 대해 읽어보신 분들은 이해하게 되실 겁니다.
바로 블록체인의 신뢰성을 이용했기 때문입니다. 물론 현재 저희가 만든 펫시터 웹은 완벽하게 해당 펫시터의 신원을 보장할 수는 없습니다.
하지만 인증서와 같은 인증 절차를 거친다면 블록체인의 취지가 더 맞아 떨어지겠죠!

그 다음으로 자신에 대한 내용을 등록해야 합니다.

![_config.yml]({{ yozzung.github.io }}/images/petsitter.png)
![_config.yml]({{ yozzung.github.io }}/images/petsitter_list.png)

그렇게 저장을 모두 마치고 나면 사용자들은 조건만 맞는다면 검색했을 때 확인할 수 있게 됩니다.
현재는 매우 간단한 형태로 저장하고 있지만 여기서 더 나아가 자세한 조건, 세부적인 내용들을 담을 수도 있습니다.

이제 사용자입장에서 저장해야할 내용입니다.
아무래도 서비스를 이용하기 위해선 자신의 펫 정보가 저장되어 있어야 합니다.

![_config.yml]({{ yozzung.github.io }}/images/enroll_pet.png)
![_config.yml]({{ yozzung.github.io }}/images/pet_list.png)

이렇게 큰 흐름의 펫시터 서비스를 위한 웹 어플리케이션 구현에 대한 설명을 마칩니다.
