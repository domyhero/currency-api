## 演示

<img data-toggle="fancybox" data-fancybox-group="gallery" href="http://yun.topthink.com/Uploads/Editor/2017-06-28/59533629e819e.png" src="http://yun.topthink.com/Uploads/Editor/2017-06-28/59533629e819e.png" alt="">

<img data-toggle="fancybox" data-fancybox-group="gallery" href="http://yun.topthink.com/Uploads/Editor/2017-06-28/5953368b00695.png" src="http://yun.topthink.com/Uploads/Editor/2017-06-28/5953368b00695.png" alt="">


## 连测试

        var socket = io("http://localhost:2345");

        setInterval(draw, 1000);

        //发送给服务器
        function draw(){
            socket.emit("api","AUDCNY");
        }

        socket.on('api', function(msg){
            var json =JSON.parse(msg);

            // console.log(json); 
        });

