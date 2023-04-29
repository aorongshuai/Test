## Canvas的应用

### Canvas画直线

```html
<canvas id="myCanvas" width="400" height="300"
        style="border:1px solid green">
</canvas>	<!--canvas边框呈现加颜色-->
<script>
    var canvas = document.getElementById("myCanvas");
    var ctx = canvas.getContext('2d');
    ctx.beginPath();
    ctx.moveTo(100,100);    /*绘制起点*/
    ctx.lineTo(200,200);    /*绘制直线*/
    ctx.strokeStyle='#000'  /*设置线条颜色*/
    ctx.lineWidth=3;        /*设置线条宽度*/
    ctx.stroke();           /*开始绘制*/
</script>
```



### Canvas直线连接出矩形

```html
<canvas id="myCanvas" width="400" height="300"
          style="border:1px solid green"></canvas>
    <script>
        var canvas = document.getElementById("myCanvas");
        var ctx = canvas.getContext('2d');
        ctx.beginPath();
        ctx.moveTo(100,100);	/*left*/
        ctx.lineTo(100,250);
        ctx.strokeStyle='green'
        ctx.stroke();
        
        ctx.beginPath();
        ctx.moveTo(100,100);	/*up*/
        ctx.lineTo(300,100);
        ctx.stroke();

        ctx.beginPath();
        ctx.moveTo(300,100);	/*down*/
        ctx.lineTo(300,250);
        ctx.stroke();

        ctx.beginPath();
        ctx.moveTo(100,250);	/*right*/
        ctx.lineTo(300,250);
        ctx.stroke();
</script>
```

### Canvas画矩形

```html
<canvas id="myCanvas" width="500" height="500" style="border: 1px solid #000"></canvas>
<script>
    var ctx = document.getElementById("myCanvas").getContext('2d');
    ctx.strokeRect(100, 100, 300, 150);	/*可重复画矩形*/
</script>
```

### Canvas填充矩形

```html
<canvas id="myCanvas" width="500" height="500" style="border: 1px solid #000"></canvas>
<script>
    var ctx = document.getElementById("myCanvas").getContext('2d');
    ctx.fillRect(100,100,300,250);	/*默认填充颜色为黑色*/
</script>
<!--填充的矩形没有绘制边框-->
```

### Canvas矩形填充颜色

```html
<canvas id="myCanvas" width="500" height="500" style="border: 1px solid #000"></canvas>
<script>
    var ctx = document.getElementById("myCanvas").getContext('2d');
    ctx.fillStyle = 'orange';   /*改变填充颜色为orange*/
    ctx.fillRect(100, 100, 300, 250);
</script>
<!--填充的矩形没有绘制边框-->
```



token：`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`

自定义域名：https://cdn.jsdelivr.net/gh/aorongshuai / PhotoTypora/repo@main
