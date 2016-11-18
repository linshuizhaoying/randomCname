#1. Usage

##1. Install randomCname.js

### npm install randomCname.js

##2. Import randomCname.js

ES6 style is supported, then get global object: randomCname.
import RandomCname from 'randomCname.js';

// or

var RandomCname = require("randomCname.js");
or link with script in html files:

<script src="randomCname.js"></script>
3. Use class RandomCname

```

 * 指定数量，性别，名字单双
 * randonCname.result(number,sex,single/double)
 * 指定姓氏数组
 * randomCname.assignLastNameArr()
 * 唯一性
 * randomCname.unique

```

```

var RandomCnameInstance = new randomCname();
//默认随机返回一个中文名
RandomCnameInstance.result()
=>["葛小凝"]

// 可按顺序指定数量,性别(male,female),单双名(single,double)
RandomCnameInstance.result(10,'female','double')

// 可生成不重复的数组
RandomCnameInstance.unique().result(10)
=>["甘英发", "明文乐", "慎英博", "元华荣", "钮弘壮", "水瑾瑜", "巫玉宇", "阴嘉悦", "刁宏大", "符英才"]

// 可指定指定姓氏数组
RandomCnameInstance.assignLastNameArr(['郑','钱']).result(10,'male','single');
=>["钱文栋", "钱雅志", "郑兴德", "郑向文", "钱学民", "郑温茂", "钱博厚", "钱修筠", "钱振海", "郑高爽"]

```


