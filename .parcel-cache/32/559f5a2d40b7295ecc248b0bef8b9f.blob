let html = document.querySelector("#html");
let style = document.querySelector("#style");
let string = `/*你好，我是一名前端新人
* 准备尝试做一个太极八卦图
* 我要开始操作div了
* 先给它添加css样式**/
body{
  font-family: PingFangSC-Light, sans-serif;
}
#div1{
  border: 1px solid rgba(0,0,0,0.3);
  width: 200px;
  height: 200px;
  box-shadow: 0 0 0 1px rgba(0,0,0,0.3);
}
/*接下来我会把div变成一个圆
* */
#div1{
  border: none;
  border-radius: 50%;
}
/*天地有混沌 八卦分阴阳
* 一黑一白
**/
#div1{
  background: linear-gradient(90deg, rgba(255,255,255,1) 0%, rgba(255,255,255,1) 50%, rgba(0,0,0,1) 50%, rgba(0,0,0,1) 50%, rgba(0,0,0,1) 100%);
}
#div1::before{
  width: 100px;
  height: 100px;
  border: 1px solid white;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  border-radius: 50%;
  background: #fff;
  background: radial-gradient(circle, rgba(0,0,0,1) 0%, rgba(0,0,0,1) 25%, rgba(255,255,255,1) 25%, rgba(252,252,252,1) 100%);
}
#div1::after{
  width: 100px;
  height: 100px;
  border: 1px solid black;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  border-radius: 50%;
  background: #000;
  background: radial-gradient(circle, rgba(255,255,255,1) 0%, rgba(255,249,249,1) 25%, rgba(0,0,0,1) 25%, rgba(0,0,0,1) 100%);
}
`;
let string2 = "";
let n = 0;

let step = () => {
  setTimeout(() => {
    if(string[n] === "\n"){
      //不照搬
      string2 += '</br>';
    }else if(string[n] === " "){
      string2 += "&nbsp;";
    }else{
      //string照搬
      string2 += string[n];
    };
    html.innerHTML = string2;
    style.innerHTML = string.substring(0, n);
    window.scrollTo(0,99999);
    html.scrollTo(0,99999);
    if(n + 1 < string.length){
    // n 不是最后一个
     n += 1 
     step();
    }else{
      // n 是最后一个
    }
  },20);
};
step();

