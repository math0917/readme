# enjoytrip 관통 프로젝트 조희라, 김원표

## html파일 설명

### index.html

![화면 캡처 2023-03-18 003004](https://user-images.githubusercontent.com/69501435/225950747-da85d415-7940-4f44-88eb-1db442d2b8f1.png)

초기 화면의 모습으로 이 중 구현에 성공한 것은 1. 지역별 여행지 2. 나의 여행 계획 페이지이다.
우선 초기 화면에서 ![스크린샷 2023-03-18 003714](https://user-images.githubusercontent.com/69501435/225951290-344ae42f-263f-4d8f-9a52-d505b5d52b49.png)
![화면 캡처 2023-03-18 003922](https://user-images.githubusercontent.com/69501435/225951749-75d52531-ebca-4370-9735-239396a26ba5.png)
나타내고 있는 것은 줄어들었을때 반응형으로 nav바가 모여있게 해줬다. 첫번째 nav인 지역별 여행지에 관한 간단한 ui를 보여주도록 설계했다.

![image](https://user-images.githubusercontent.com/69501435/225952374-7e4a0090-9ca7-4e1c-a183-b09c3cb8bc1e.png)

이 경우 전국 관광지를 들고올때 사용자가 부산을 선택하면 부산에 해당하는 시군구를 fetch받을 수 있도록 하였고 최종적으로 도와 시군구와 contentType으로 data를 fetch받고 핀을 찍을 수 있도록 한다.

![image](https://user-images.githubusercontent.com/69501435/225953367-27af93b4-edf1-4570-8169-7fe1fdee40be.png)
사용자가 검색을 하고 핀을 눌렀을때 관련 정보를 사용자가 볼 수 있도록 하였다. 밑에는 관련된 정보를 나열해 놓았습니다. 만약 밑에 그 장소에 해당하는 열을 누를 시 그 곳의 위도와 경도를 가운데 값으로 하는 시야를 보여주도록 설계했습니다.
![image](https://user-images.githubusercontent.com/69501435/225954001-e559b8a8-1bdd-46f5-a683-84921707328f.png)

![image](https://user-images.githubusercontent.com/69501435/225954193-d0f73505-e176-4e8d-a7e0-924e2caf3bd6.png)
나의 여행계획 페이지이다. 이 페이지의 경우 키워드로 해당 키워드를 가진 모든 요소를 리스트로 보여준다.

![image](https://user-images.githubusercontent.com/69501435/225954373-c51c15cc-7237-46e8-872e-44360d0c591e.png)
그 후 가고 싶은 곳들을 눌러보며 그 주위에 무엇이 있는지 확인하고 만약 마음에 들면 핀을 한번더 클릭한다.
![image](https://user-images.githubusercontent.com/69501435/225955241-2ab37a43-939b-4a2b-8d54-9c94e33b9e83.png)

회원가입 페이지는 modal로 구성했다.
![image](https://user-images.githubusercontent.com/69501435/225955505-b62b1c5c-928b-499c-9495-eeee4921b6dd.png)

로그인 또한 modal로 구성했다.
![image](https://user-images.githubusercontent.com/69501435/225956245-b1778e8d-5edf-4c82-8031-1ec749ec53d9.png)

로그인 후 화면의 모습이다.
![image](https://user-images.githubusercontent.com/69501435/225956470-9b624532-440d-4feb-8d0f-5106dcc6ee15.png)

마이페이지를 누르면 내부에 나의 정보가 적혀있다. 이 중 일부를 수정하고 수정을 누르면 수정이 완료된다.
![image](https://user-images.githubusercontent.com/69501435/225956627-d905b6b6-0691-4de3-980e-51d4edac581a.png)

로그아웃을 누르면 초기의 상태로 돌아간다. 이는 db가 존재하지 않아 localstorage의 flag를 줌으로써로그인이 되어있는지, 로그아웃이 되어있는지 표현했다.
![image](https://user-images.githubusercontent.com/69501435/225956717-0a355f20-bb39-42e2-83d5-32aed1745a6b.png)

핫플자랑하기와 여행정보공유는 아직 구현하지 않았다.

+++ 추가된 사항
나의 여행 계획 페이지에서 추가하기 버튼을 추가하였다. + 추가하기 버튼을 누르면 모달창으로 추가할 수 있도록 하였다.
![image](https://user-images.githubusercontent.com/69501435/226165969-febea032-1f49-43af-991f-bf60b0f93389.png)
![image](https://user-images.githubusercontent.com/69501435/226165981-5b8f388c-82ba-41e9-ab9f-232bb69841d6.png)

핫플자랑하기 페이지에 게시글을 올릴수 있도록 ui를 만들었다.
![image](https://user-images.githubusercontent.com/69501435/226166049-7b15198f-5d55-40b8-9b1b-917ef95662d0.png)
여행정보공유페이지 또한 ui를 만들었고, 이후에 글쓰기 기능을 db가 생기고 나면 추가할 계획이다.
![image](https://user-images.githubusercontent.com/69501435/226166056-cde9c899-0d0e-42e5-a817-9fc716955d89.png)


회원 탈퇴 기능은 마이페이지에서 만약 탈퇴를 누르면
![image](https://user-images.githubusercontent.com/69501435/226172843-f524b4d8-e99a-4d96-8f68-b0bdd5180b16.png)
기존에 로그인이 풀리고 로컬스토리지에서 저장되있던 유저 데이터가 사라지게된다.
![image](https://user-images.githubusercontent.com/69501435/226172862-2532e6c0-c4a4-4629-b101-52ecd2b29987.png)



