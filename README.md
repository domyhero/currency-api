##链接

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

