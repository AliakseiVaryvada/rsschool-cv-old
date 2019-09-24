## ["Markdown & Git"][1]
[1]: https://github.com/rolling-scopes-school/tasks/blob/master/tasks/git-markdown.md
## Varyvada Aliaksei
## Contact Info:
#### Telephone nuber: +375 (33) 3037269
#### E-mail: alv96@bk.ru
## Summary 
Hello, my name is Aliaksei Varyvada. I am 23 years old. I am energetic and quickly trained person. A wide-profile specialist with straight arms and a smart head. Without bad habbits. Knowledge and understanding of computer industry development trends. I am interested in IT, knowledge of the basics of programming (C ++, JAVA, HTML5, CSS, JS), desire to work in this industry. My objective is to start a career with a junior in EPAM Systems and get further development here.
## Skills 
* HTML (base);
* CSS (base);
* JS (base);
* Java (base);
* Photoshop, Coral Draw;
* Repair all kinds of the electronic device.
## Code examples

* Codewars [Kata][2].

[2]: https://www.codewars.com/kata/the-observed-pin/train/javascript "Codewars"

<details>
  
<summary>Code</summary>

```javascript
  function getPINs(observed) {
    let arrR = [];
    let l = [...observed];
    for(let k = 0; k<l.length; k++){
        console.log(l[k]);
        switch (l[k]) {
            case '1' :
                arrR.push(['1', '2', '4']);
                break;
            case '2' :
                arrR.push(['1', '2', '3', '5']);
                break;
            case '3' :
                arrR.push(['3', '2', '6']);
                break;
            case '4' :
                arrR.push(['4', '1', '7', '5']);
                break;
            case '5' :
                arrR.push(['5', '2', '8', '4', '6']);
                break;
            case '6' :
                arrR.push(['6', '3', '9', '5']);
                break;
            case '7' :
                arrR.push(['7', '4', '8']);
                break;
            case '8' :
                arrR.push(['8', '5', '0', '7', '9']);
                break;
            case '9' :
                arrR.push(['9', '8', '6']);
                break;
            case '0' :
                arrR.push(['0', '8']);
                          break;
        }
    }
   function allPossibleCases(arr) {
        if (arr.length == 1) {
            return arr[0];
        } else {
            var result = [];
            var allCasesOfRest = allPossibleCases(arr.slice(1));  // recur with the rest of array
            for (var i = 0; i < allCasesOfRest.length; i++) {
                for (var j = 0; j < arr[0].length; j++) {
                    result.push(arr[0][j] + allCasesOfRest[i]);
                }
            }
            return result;
        }
        return result;
    }
   let arrItog = allPossibleCases(arrR);
   return (arrItog);
}  
```  
</details>
