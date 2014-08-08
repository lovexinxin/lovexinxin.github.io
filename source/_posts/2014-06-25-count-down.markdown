---
layout: post
title: "Count Down"
date: 2014-06-25 00:45:05 -0400
comments: true
categories: 
---
<script language="Javascript" type="text/javascript">
			var clock;

			$(document).ready(function() {

				// Grab the current date
				var currentDate = new Date();

				// Set some date in the future. In this case, it's always Jan 1
				// var futureDate  = new Date(currentDate.getFullYear() + 1, 0, 1);
				var futureDate = new Date("2014/08/18 22:30:00")

				// Calculate the difference in seconds between the future and current date
				var diff = futureDate.getTime() / 1000 - currentDate.getTime() / 1000;

				// Instantiate a coutdown FlipClock
				clock = $('.clock').FlipClock(diff, {
					clockFace: 'DailyCounter',
					countdown: true,
					showSeconds: false
				});
			});
</script>

# Tick tick ...
希望我们能努力跑赢这个倒计时牌，能够坚持下来，坚持到我们的“Unofficial Honeymoon”...
<div class="clock" style="margin:2em;"></div>