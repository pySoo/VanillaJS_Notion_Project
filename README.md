# VanillaJS 노션 클로닝 프로젝트

## 🌐 Demo

https://github.com/prgrms-fe-devcourse/FEDC5-5_Project_Notion_VanillaJS/assets/55135881/9dbfe355-a043-4c90-a591-23efb1b73473

<br />

## 🏠 프로젝트 구조

1. 반복되는 [DOM 생성 로직](https://github.com/pySoo/VanillaJS_Notion_Project/blob/main/src/utils/dom.js#L8)을 tag, props, children props를 이용하여 추상화
2. [CSS selector 상수화](https://github.com/pySoo/VanillaJS_Notion_Project/blob/main/src/components/SideBar.js#L10)
   - DOM을 selecting하는 부분과 DOM 생성시 클래스를 주입하는 부분이 100% 일치
   - 미스매치로 인한 버그 방지
3. Sidebar 트리 구조를 [재귀 함수를 이용하여 추상화](https://github.com/pySoo/VanillaJS_Notion_Project/blob/main/src/utils/dom.js#L22)
4. history API를 이용한 [SPA 구현](https://github.com/pySoo/VanillaJS_Notion_Project/blob/main/src/routes/router.js)
5. [로컬 스토리지 사용 가능 여부를 검사](https://github.com/pySoo/VanillaJS_Notion_Project/blob/main/src/utils/canUseStorage.js)하는 함수를 추상화

<br />

## 📦 파일 구조

```
📦 src
├── 📂 assets
|── 📂 components
|   ├── 📂 Common
|   ├── 📂 Document
|   ├── 📂 Editor
|   └── 📂 MyWorkSpace
├── 📂 constants
├── 📂 pages
├── 📂 routes
├── 📂 service
├── 📂 styles
└── 📂 utils
```
