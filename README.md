# 발견 문제점
## 1. write.jsp 에서 에러 발생

> **원인** : write.jsp에서 if문안 누락발생

```java
	if(name == ""){
		alert("작성자 란은 반드시 입력해야 합니다");
		frm['name'].focus();  ===> ${list[0].regDate}
    }
        --->
    	if(name == ""){
		alert("작성자 란은 반드시 입력해야 합니다");
		frm['name'].focus();
		return false;
	}


```