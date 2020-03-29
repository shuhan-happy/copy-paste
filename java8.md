字符串数组转Long数组

	List<Long> list = Arrays.asList(StringUtils.split(commentIds, ",")).stream().map(NumberUtils::toLong).collect(Collectors.toList());
