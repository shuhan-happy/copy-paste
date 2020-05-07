###LocalDate

    // 当前日期的月份的第一天
    LocalDate firstDay = LocalDate.now().withDayOfMonth(1);

    // 当前日期的月份的第一天 是周几
    int firstDayOfWeek = LocalDate.now().getDayOfWeek().getValue();

    // 当前日期的月份的最后一天
    LocalDate endDay = LocalDate.now().withDayOfMonth(LocalDate.now().lengthOfMonth());

    // 日历上展示的第一天
    LocalDate calendarStartDay = firstDay.minusDays(firstDayOfWeek - 1);

    // 日历上展示的最后一天
    LocalDate calendarLastDay = endDay.plusDays(7 - endDay.getDayOfWeek().getValue());

    // 当前日期的周一
    LocalDate monday = LocalDate.now().with(DayOfWeek.MONDAY);
	
	
###LocalDateTime

	// 两个时间间隔几个小时
	Duration dur = Duration.between(answerDateTime, LocalDateTime.now());
	long hours = dur.toHours();
	
###convert

	LocalDateTime localDateTime = LocalDate.now().atStartOfDay();	
