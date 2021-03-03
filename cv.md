<h1>Zmiyevskaya Anna</h1>
<p>Woman, 21, was born 11.05.1999</p>
<p></p>
<p>+7 (950) 0192079</p>
<p>annazmei2014@gmail.com</p>
<p>github: https://github.com/nyamzmeya</p>
<p></p>
<p>Place of living: Saint-Petersburg</p>
<p>Citizenship: Kazakhstan</p>

<h1>Career objective</h1>
<p>Junior Frontend-developer</p>
<p>I want to develop cool interfaces, develop programming skills, learn new technologies</p>
<p>Example code: calculator function. The function accepts arithmetic operations on two numbers
(Arabic or Roman numbers) as a string and returns a string with the result of their execution</p>

```
function calculator(string) {
const str = string;
const dic = {"I" : 1,"II" : 2,"III" : 3,"IV" : 4,"V" : 5,"VI" : 6,"VII" : 7,"VIII" : 8,"IX" : 9, "X" : 10};

const re = new RegExp("\\b(" + Object.keys(dic).join("|") + ")\\b","gi");

const str2 = str.replace(re, function(matched){
return dic[matched];});

const numbers2 = str2.match(/\d+/g).map(Number);
const numbers = str.match(/\d+/g);
const sign = str2.match(/[+-/*]/g);
const cond = ((sign == '+' || sign == '-' || sign == '*' || sign == '/') && numbers2[0] <= 10 && numbers2[1] <= 10 && (numbers2[0] != 0 && numbers2[1] != 0));

if (cond && numbers == null && numbers2.length == 2) {
if (calculator2(numbers2, sign) > 0 ) {
return toRoman(calculator2(numbers2, sign));
} else return '';
} else if (cond && numbers.length == 2) {
return String(calculator2(numbers2, sign));
} else throw "Error";
}

function toRoman(num) {
const toroman = {"C": 100, "XC": 90, "L": 50, "XL": 40,
"X" : 10, "IX" : 9, "V" : 5, "IV" : 4, "I" : 1}
let roman = '';
for (const key in toroman) {
while (num >= toroman[key]) {
roman += key;
num -= toroman[key];
}
}
return roman;
}

function calculator2(numbers, sign1) {
let res;
if (sign1 == '+') {
res = numbers[0] + numbers[1];
} else if (sign1 == '-') {
res = numbers[0] - numbers[1];
} else if (sign1 == '*') {
res = numbers[0] * numbers[1];
} else if (sign1 == '/') {
res = numbers[0] / numbers[1];
}
return Math.trunc(res);
}
```

<h1>Education</h1>
<p>Incomplete higher education</p>
<p>Year graduation: 2022</p>
<p>National Research University Higher School of Economics</p>
<p>Social Sciences, Political Science and World Politics</p>
<p>Courses Completed: Web Developer 2021 (Udemy)</p>

<h1>Key skills</h1>
<p>Russian - Native</p>
<p>English - B2</p>
<p>German - A1</p>
<p>Skills: Execution, React, CSS, HTML, Sass, Gulp, Bootstrap, JavaScript, Python, R, Git</p>
