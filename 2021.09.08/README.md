# imagineer_project
졸업작품
### 2021.09.08 일지     
학교에서 회의를 하고 각자 역할 분담을 했다.   
내 역할은 글쓰기(+수정,삭제) 그리고 상세 페이지 담당이다.   
이번 주는 일단 간단히 폼을 그리기로 했다.   
     
 방학 때 GSITM에서 배웠던 내용이 손에 익어서 그런지 금방 끝났다.   
    
 remove.html에서 remove()함수를 원래 delete()함수로 했었는데 delete는 원래 지정되어있는 함수여서 사용하지 못한다는 에러를 보고 remove()로 바꿨다.   
 오늘 처음 알게 되었다. 코딩은 이론으로 하는 것보다 실제로 해야 공부 된다는 것을 오늘 다시 한 번 느꼈다.   
    
 사진을 input type을 image로 해서 하면 업로드 창이 나올 줄 알았는데, 생각처럼 되지 않았다. 그 부분은 공부해서 수정해야 할 거 같다.   
      
 write.html은 글쓰기   
 modify.html은 글 수정 페이지   
 remvoe.html은 글 삭제 페이지 
 
write.html  
```
<!DOCTYPE html>
<html>
<head>
<title>생파</title>
</head>
<body>

<h1>상품등록</h1>
<hr class="one">
<tr>
    <td>상품명 <input type="text" id="name" name="name" placeholder="상품명을 입력하세요"></td>
</tr>
<br>
<tr>
    <td>카테고리 
        <select name="category" id="category">
        <option value="1";>곡류</option>
        <option value="2";>과일류</option>
        <option value="3";>버섯류</option>
        <option value="4";>채소</option>
        <option value="5";>견과류</option>
        <option value="6";>기타 농산물</option>
    </select></td>
</tr>
<br>
<tr>
    <td>가격 <input type="number" id="price" name="price" placeholder="가격을 입력하세요"></td>원
</tr>
<br>
<tr>
    <td>사진 <input type="image" id="image" name="image"></td>
</tr>
<br>
<tr>
    <td>유튜브 URL <input type="url" id="url" name="url" placeholder="해당 주소를 입력하세요"></td>
</tr>
<br>
<tr>
    <td>유튜브 이미지 <input type="image" id="uimage" name="uimage" ></td>
</tr>
<br>
<tr>
    <td>상세 정보 <br> <input type="text" id="contents" name="contents" placeholder="상세 정보를 입력하세요"></td>
</tr>
<br>
<div style="text-align: right;">
    <button onclick="save()">등록</button>
    <button onclick="cancel()">취소</button>
</div>
<script>
    function save()
    {
        alert('등록되었습니다');
        location.href='list.html';
    }
    function cancel()
    {
        alert('취소되었습니다');
        location.href='list.html';
    }
</script>

</body>
</html>
```
modify.html   
```
<!DOCTYPE html>
<html>
<head>
<title>생파</title>
</head>
<body>

<h1>수정</h1>
<hr class="one">
<tr>
    <td>상품명 <input type="text" id="name" name="name" placeholder="상품명을 입력하세요"></td>
</tr>
<br>
<tr>
    <td>카테고리 
        <select name="category" id="category">
        <option value="1";>곡류</option>
        <option value="2";>과일류</option>
        <option value="3";>버섯류</option>
        <option value="4";>채소</option>
        <option value="5";>견과류</option>
        <option value="6";>기타 농산물</option>
    </select></td>
</tr>
<br>
<tr>
    <td>가격 <input type="number" id="price" name="price" placeholder="가격을 입력하세요"></td>원
</tr>
<br>
<tr>
    <td>사진 <input type="image" id="image" name="image"></td>
</tr>
<br>
<tr>
    <td>유튜브 URL <input type="url" id="url" name="url" placeholder="해당 주소를 입력하세요"></td>
</tr>
<br>
<tr>
    <td>유튜브 이미지 <input type="image" id="uimage" name="uimage" ></td>
</tr>
<br>
<tr>
    <td>상세 정보 <br> <input type="text" id="contents" name="contents" placeholder="상세 정보를 입력하세요"></td>
</tr>
<br>
<div style="text-align: right;">
    <button onclick="modify()">수정</button>
    <button onclick="cancel()">취소</button>
</div>
<script>
    function modify()
    {
        alert('수정되었습니다');
        location.href='list.html';
    }
    function cancel()
    {
        alert('취소되었습니다');
        location.href='list.html';
    }
</script>

</body>
</html>
```
remove.html
```
<!DOCTYPE html>
<html>
<head>
<title>생파</title>
</head>
<body>

<h1>삭제</h1>
<hr class="one">
<tr>
    <td>상품명 <input type="text" id="name" name="name" placeholder="상품명을 입력하세요"></td>
</tr>
<br>
<tr>
    <td>카테고리 
        <select name="category" id="category">
        <option value="1";>곡류</option>
        <option value="2";>과일류</option>
        <option value="3";>버섯류</option>
        <option value="4";>채소</option>
        <option value="5";>견과류</option>
        <option value="6";>기타 농산물</option>
    </select></td>
</tr>
<br>
<tr>
    <td>가격 <input type="number" id="price" name="price" placeholder="가격을 입력하세요"></td>원
</tr>
<br>
<tr>
    <td>사진 <input type="image" id="image" name="image"></td>
</tr>
<br>
<tr>
    <td>유튜브 URL <input type="url" id="url" name="url" placeholder="해당 주소를 입력하세요"></td>
</tr>
<br>
<tr>
    <td>유튜브 이미지 <input type="image" id="uimage" name="uimage" ></td>
</tr>
<br>
<tr>
    <td>상세 정보 <br> <input type="text" id="contents" name="contents" placeholder="상세 정보를 입력하세요"></td>
</tr>
<br>
<div style="text-align: right;">
    <button onclick="remove()">삭제</button>
    <button onclick="cancel()">취소</button>
</div>
<script>
    function remove()
    {
        alert('삭제되었습니다');
        location.href='list.html';
    }
    function cancel()
    {
        alert('취소되었습니다');
        location.href='list.html';
    }
</script>

</body>
</html>
```

