![header](https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=Toy_Project&fontSize=60)

# Toy Project

### [프로젝트 기간]
-

### [기술 스택]
<img src="https://img.shields.io/badge/Unreal Engine-000000?style=flat-square&logo=Unreal Engine&logoColor=white"/>  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=C++&logoColor=white"/>  <img src="https://img.shields.io/badge/Blueprint-137CBD?style=flat-square&logo=Blueprint&logoColor=white"/>

### [아키텍처]
-

### [프로젝트 내용]
3인칭 FPS / 카드게임 / 각종 이펙트 등 1인 개발 토이 프로젝트입니다.

<img width="30%" src="https://user-images.githubusercontent.com/90584581/197500588-65c33b88-0cd0-467d-9dc0-9e52e25c39d4.png"/>  <img width="30%" src="https://user-images.githubusercontent.com/90584581/197500597-d9a12ac5-efc8-451e-ae45-a117d764dcba.png"/>  <img width="30%" src="https://user-images.githubusercontent.com/90584581/197500600-d36ebeb5-5323-4042-8214-a5dceb62cd6e.png"/>
<img width="30%" src="https://user-images.githubusercontent.com/90584581/197500607-226473b3-48a5-4bf0-a8e4-bca057cfa75e.png"/>  <img width="30%" src="https://user-images.githubusercontent.com/90584581/197500611-41fd1c62-b6e9-4f38-be68-872050d7cb6c.png"/>  <img width="30%" src="https://user-images.githubusercontent.com/90584581/197500612-b594b313-577c-4586-9bb4-668a2135d823.png"/>
<img width="30%" src="https://user-images.githubusercontent.com/90584581/197500570-49ce4798-e347-48ec-9562-b06c990e18ce.png"/>  <img width="30%" src="https://user-images.githubusercontent.com/90584581/197500575-832d327d-259f-4e77-833f-75cb3d52f0d5.png"/>  <img width="30%" src="https://user-images.githubusercontent.com/90584581/197500582-80822f34-cbe6-49db-83ab-bc7aadbc9bd1.png"/>

### [프로젝트 투입 인원]
개발자 1

## [주요 코드]
### [먼저 3인칭 FPS 코드 분석입니다.]
#### Fire
Fire 기능은 "Set Timer By Event" 함수를 이용해 연사가 가능하게 했으며 "LineTraceForObject"함수를 통해 데미지 처리를 했습니다.\
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197504178-d04f3899-14ef-4438-a754-0741a62f6605.png"/>
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197504184-5a40cb97-85bd-44f9-b11b-4aac2217c126.png"/>

#### Reload
Reload 기능은 몽타주 기능을 이용하여 본의 "Spine"을 기준으로 상체만 Reload 애니메이션되게 구현했습니다.
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197505019-1d03c790-e841-460f-91ad-8e94dbb0ec3c.png"/>


#### Weapon Drop
무기는 Datatable로 지정 위치에 생성되도록 기능을 구현하였습니다.
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197505787-77d59a8e-6fa8-4e5f-bdbf-49db4e6e0e62.png"/>
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197505779-99ca8ce8-c0de-42fc-b103-4c0b822fe13e.png"/>

#### AI
AI를 구성하는 Behavior Tree입니다. NPC 시야 안에 있거나 주변에서 소리를 인식하면 캐릭터를 향해 따라오며 사격합니다.\
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197506060-e2859e26-5b51-4ca9-aa2d-1ce7f9b8ce1b.png"/>


### [다음으로 Card Game 코드 분석입니다.]
#### Spawn Random location
카드들이 지정된 자리에 랜덤하게 스폰되도록 구현했습니다.
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197508330-c8ae11a0-19b3-4a30-b4f1-e7460480f817.png"/>

#### Number Compare
각 카드별로 정해져있는 고유 넘버를 통해서 비교하고 맞으면 사라집니다.
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197508567-bd6ffe0e-c9ec-4b63-a43d-c0415f083509.png"/>

### [마지막으로 VFX 코드 분석입니다.]
#### World outline
대상의 Outline만을 렌더링해주는 머티리얼을 설정하고 "PostProcessVolume"에 적용한 후 캐릭터에서 머티리얼의 파라미터를 조절하여 구현했습니다.\
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197510087-c8036fd7-4669-46e8-ab88-a80556641a83.png"/>
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197510187-441c589c-4d19-4819-ace0-146619ae787d.png"/>

#### Teleport
마우스 커서의 Hit result location을 통해서 Path를 만들어주고 그곳을 따라 움직이도록 설정했습니다. 도착시 이펙트가 터집니다.\
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197510844-9bb9d51c-d28b-4e46-9b0b-0f7c620f3886.png"/>
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197510838-a46ea943-4ebc-4198-9be1-51bed3497b6f.png"/>

#### Character Effect
Niagara Particle System을 이용하여 지정된 캐릭터의 본 위치에 파티클이 생성되도록 구현했습니다.
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197511174-866db9c5-c298-4e4c-891d-4c0f0b5cc639.png"/>
<img width="60%" src="https://user-images.githubusercontent.com/90584581/197511183-418b5156-9993-46a1-9f99-60cfcc49d8cb.png"/>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=footer)
