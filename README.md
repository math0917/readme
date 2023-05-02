# enjoy trip spring 공민혁, 기대성, 김원표

## board(게시판 부분 crud)

### Create
![Image Pasted at 2023-5-2 17-47](https://user-images.githubusercontent.com/69501435/235645428-25e99d29-f794-45a1-988e-5a895ded4ad3.png)

uri : /board
method : POST
body는 json형태로 제공한다.

response는 상태코드가 201이라면 created, int값은 이번에 추가한 insert의 id값이다.

### Read
![Image Pasted at 2023-5-2 17-44](https://user-images.githubusercontent.com/69501435/235646115-0941272d-2c8b-4783-a538-bdb47065efb7.png)

uri : /board/{id}
method : GET
path variable로 글 상세보기를 지원한다.

response는 글에 대한 상세정보가 포함된다. 

### List
![Image Pasted at 2023-5-2 17-44 (1)](https://user-images.githubusercontent.com/69501435/235646547-e8d5538c-d2ae-4ab8-b954-e670a5a720ad.png)

uri : /board
method : GET
글 리스트를 반환받는다.

response에는 json형태의 데이터를 포함하는 리스트가 받아진다.
