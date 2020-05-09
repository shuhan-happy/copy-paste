字符串数组转Long数组

	List<Long> list = Arrays.asList(StringUtils.split(commentIds, ",")).stream().map(NumberUtils::toLong).collect(Collectors.toList());

list转map

	accounts.stream().collect(Collectors.toMap(Account::getUsername, Function.identity(), (key1, key2) -> key2));
