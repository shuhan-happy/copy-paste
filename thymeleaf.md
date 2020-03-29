输出文本

	  <p th:text="${moment.text}">评论内容</p>

遍历list

	<th th:each="userhead : ${userhead}" th:text="${userhead.key}"></th>
