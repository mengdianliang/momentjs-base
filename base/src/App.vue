<template>
  <div id="app">
    <a href='http://momentjs.cn/docs/#/plugins/'>http://momentjs.cn/docs/#/plugins/</a>
    <ul>
      <li>{{date}}</li>
      <li>{{date1}}</li>
      <li>{{date2}}</li>
      <li>{{date3}}</li>
      <li>{{date4}}</li>
      <li>{{date5}}</li>
      <li>{{date6}}</li>
      <li>{{date7}}</li>
      <li>{{date8}}</li>
    </ul>
  </div>
</template>

<script>
import moment from 'moment'
export default {
  name: 'app',
  components: {},
  data () {
    return {
      // 当前时间
      date: moment(),
      date1: '',
      date2: '',
      date3: '',
      date4: '',
      date5: '',
      date6: '',
      date7: '',
      date8: ''
    }
  },
  mounted () {
    // moment({ hour: 15, minute: 10 });
    // moment({ y: 2010, M: 3, d: 5, h: 15, m: 10, s: 3, ms: 123 });
    // moment({ year: 2010, month: 3, day: 5, hour: 15, minute: 10, second: 3, millisecond: 123 });
    // moment({ years: 2010, months: 3, days: 5, hours: 15, minutes: 10, seconds: 3, milliseconds: 123 });
    // moment({ years: 2010, months: 3, date: 5, hours: 15, minutes: 10, seconds: 3, milliseconds: 123 });

    // moment().millisecond(Number);
    // moment().millisecond(); // Number
    // moment().milliseconds(Number);
    // moment().milliseconds(); // Number

    // moment().second(Number);
    // moment().second(); // Number
    // moment().seconds(Number);
    // moment().seconds(); // Number

    // moment().minute(Number);
    // moment().minute(); // Number
    // moment().minutes(Number);
    // moment().minutes(); // Number

    // moment().hour(Number);
    // moment().hour(); // Number
    // moment().hours(Number);
    // moment().hours(); // Number

    // moment().date(Number);
    // moment().date(); // Number
    // moment().dates(Number);
    // moment().dates(); // Number

    // moment().day(Number|String);
    // moment().day(); // Number
    // moment().days(Number|String);
    // moment().days(); // Number

    // moment().month(Number | String);
    // moment().month(); // Number
    // moment().months(Number | String);
    // moment().months(); // Number

    // moment().quarter(); // Number
    // moment().quarter(Number);

    // moment().year(Number);
    // moment().year(); // Number
    // moment().years(Number);
    // moment().years(); // Number

    // moment().add(Number, String);
    // moment().add(Duration);
    // moment().add(Object);

    // moment([2010, 0, 31]);                  // January 31
    // moment([2010, 0, 31]).add(1, 'months'); // February 28

    // moment().subtract(Number, String);
    // moment().subtract(Duration);
    // moment().subtract(Object);

    // 通过将原始时刻设置为单位时间的开始来突变原始时刻。
    // moment().startOf('year');    // set to January 1st, 12:00 am this year
    // moment().startOf('month');   // set to the first of this month, 12:00 am
    // moment().startOf('quarter');  // set to the beginning of the current quarter, 1st day of months, 12:00 am
    // moment().startOf('week');    // set to the first day of this week, 12:00 am
    // moment().startOf('isoWeek'); // set to the first day of this week according to ISO 8601, 12:00 am
    // moment().startOf('day');     // set to 12:00 am today
    // moment().startOf('hour');    // set to now, but with 0 mins, 0 secs, and 0 ms
    // moment().startOf('minute');  // set to now, but with 0 seconds and 0 milliseconds
    // moment().startOf('second');  // same as moment().milliseconds(0);

    // moment().endOf("year"); // set the moment to 12-31 11:59:59.999 pm this year

    // moment().format();                                // "2014-09-08T08:02:17-05:00" (ISO 8601)
    // moment().format("dddd, MMMM Do YYYY, h:mm:ss a"); // "Sunday, February 14th 2010, 3:25:50 pm"
    // moment().format("ddd, hA");                       // "Sun, 3PM"
    // moment('gibberish').format('YYYY MM DD');         // "Invalid date"

    this.date1 = moment('1995-12-25').format('MMMM Do YYYY, h:mm:ss a')
    this.date2 = moment().format('dddd')
    this.date3 = moment().format('MMMM Do YY')
    this.date4 = moment().format('YYYY [escaped] YYYY')
    this.date5 = moment().format()
    // this.date6 = moment("12-25-1995", "MM-DD-YYYY");
    this.date7 = moment(new Date(2011, 9, 16))
    this.date8 = moment([2010, 1, 14, 15, 25, 50, 125])
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
