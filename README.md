# snakeAI
🚀A snake AI written in JavaScript，based on BFS&amp;DFS Algorithm✨✨✨

<font size=70>[查看demo](https://jarrelljiang.github.io/snakeAI/")</font>

如果在中期，蛇头走最远路线追蛇尾时，假如虚拟蛇走完下一步会形成一个孤立的空格，则实际蛇走距蛇头第二远的那一格。  
可以把4个方向中能走的路线方向放入一个数组，按从长到短排，最长的会形成孤立空格的话就走第二长的。  
如果数组里面就一个方向，那就只能直接走这个方向了。
    
    var arr=['a','abc','ab']
    arr.sort((a,b)=>b.length-a.length)
    console.log(arr) //  ["abc", "ab", "a"]
![avatar](https://github.com/jarrelljiang/snakeAI/blob/master/images/1.png?raw=true)
比如蛇吃完圈中的食物后是向右走的，但是形成了空格，这时候不应该向右，而是走第二远的点，也就是向下。

