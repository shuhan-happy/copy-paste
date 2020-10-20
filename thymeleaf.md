输出文本

	  <p th:text="${moment.text}">评论内容</p>

遍历list

	<th th:each="userhead : ${userhead}" th:text="${userhead.key}"></th>
	
图片

	<img th:src="@{/qm/common/wx/qrcode?path=pages%2Fauth%2Fauth&width=300&scene=a}" src="#" class="qrcode"/>	

添加class

	<a href="" class="baseclass" th:classappend="${isAdmin} ? adminclass : userclass"></a>

读取url里的参数

	${param.foo}
