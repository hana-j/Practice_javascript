# javascript practice


## Variable 선언
* let : 변할 수 있는 값
* const : 상수 
----------
## clock.js 스크립트 구현 순서 
1. Create function init(){}, init();
   ```
   function init(){
        getTime();
        setInterval(getTime, 1000);
    }
    init();

2. html 문서 내의 태그를 지정하는 변수 선언 
    ```
    const clockContainer = document.querySelector(".js-clock");
    ```
3. 필요한 데이터를 불러올 함수 선언 
    ```
    function getTime(){
        const date = new Date();
        const minutes = date.getMinutes();
        const hours = date.getHours();
        const seconds = date.getSeconds();
        clockTitle.innerText = 
        `${hours<10?`0${hours}`:hours}:
        ${minutes<10?`0  {minutes}`:minutes}:
        ${seconds<10 ?`0${seconds}` : seconds
    }`;
    ```

