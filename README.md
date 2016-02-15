# Clock-degrees
HackerRank Challenge for FS Test
function clockCalc(hour, minute) {
    hour = (hour % 12) * 30 + minute / 60 * 30;
    minute = minute * 6;
    console.log(hour);
    console.log(minute);
    var max = Math.max(hour,minute);
    var min = Math.min(hour,minute);
    return Math.min(max-min,360-max+min);
}
clockCalc(6, 5)
