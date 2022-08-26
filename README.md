<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>网上办事大厅-校园通行卡</title>
    <style>
        body{
            margin: 0;
            font-family: 'Courier New', Courier, monospace;
        }
        .box{
            height: 800px;
            width: 528px;
            background-color:#6bc372;
            position: fixed
        }
        .choose_box{
            margin-top: 10px;
        }
        .choose_1{
            display: inline-block;
            height: 42px;
            width: 100px;
            background-color: white;
            text-align: center;
            line-height: 45px;
            border: 1px solid gray;
            position: absolute;
            top: 15px;
            right: 30.8%;
            color: gray;
            border-radius: 0 5px 5px 0;
            
        }

        .choose_2{
            display: inline-block;
            height: 42px;
            width: 100px;
            line-height: 45px;
            background-color: white;
            text-align: center;
            border: 1px solid gray;
            position: absolute;
            top: 15px;
            left: 30.8%;
            color: gray;
            border-radius: 5px 0 0 5px;
        }

        .choose_1:hover{
            color: white;
            border: solid #669bcf 1px;
            background-color: #1e5193;
            
        }

        .choose_2:hover{
            color: white;
            border: solid #669bcf 1px;
            background-color: #1e5193;
        }

        .white_bj{
            display: block;
            position: fixed;
            top: 70px;
            left: 65px;
        }

        #beijing{

            position: fixed;
            top: 90px;
            left: 38%;
            
        }
        
        #enter_name{
            position: fixed;
            top: 90px;
            left: 44%;
        }


        .cut_line_1{
            height: 1px;
            width: 320px;
            background-color: rgb(220, 220, 220);
            position: fixed;
            top: 170px;
            left: 18.5%;
        }

        #jjl{
            position: fixed;
            top: 212px;
            left: 34%;
        }

        img{
            border-radius: 10px;
        }

        #green_line{
            position: fixed;
            top: 190px;
            left: 32%;
        }
        
        .guest_information{
            font-style: none;
            position: fixed;
            top: 400px;
            left: 25%;
        }

        ul{
            text-decoration: none;
            list-style: none;
            line-height: 25px;
            font-size: 12px;
            position: fixed;
            left: 155px;
        }
        .w-title{
            color: gray;
            width: 40px;
        }

        table{
            font-size: 12px;
            position: fixed;
            top: 411px;
            line-height: 21px;
            right: 210px;
            color: rgb(77, 76, 76);
        }

    
        .cut_line_2{
            height: 1px;
            width: 320px;
            background-color: rgb(220, 220, 220);
            position: fixed;
            top: 595px;
            left: 18.5%;
        }

        #passport{
            font-size: 20px;
            color: #38ac41;
            display: block;
            position: fixed;
            top: 600px;
            left: 220px;
            font-weight: 500;
        }

			.showTime {
                display: block;
                width: 320px;
                height: 35px;
                background-color: #ecf5ee;
                position: fixed;
                top: 130px;
                left: 18.5%;
                border-radius: 10px;
                text-align: center;
                line-height: 40px;
                color: #6bc372;
				text-align: center;
			}
        
            #bottom{
                position: fixed;
                top: 515px;
            }
    </style>
</head>
<body>
    <div class="box">
        <div class="choose_box">
            <span class="choose_1" onclick=editinPut(1) >入校码</span>
            <span class="choose_2" onclick=editinPut(2) >出校码</span>
        </div>
        <div class="health_box">
            <span class="white_bj">
                <img src="./图片/bgjian.aa1b69b4.png" alt="" width="400px">
            </span>
            <div class="health_box_title">
                <span id="beijing">
                    <img src="./图片/WechatIMG3128.jpeg" alt="" width="25px">
                </span>
                <span id="enter_name"></span>
            </div>
            <div class="showTime">
                <span id="auto-refresh-date">2021年10月08日</span>
                <span id="auto-refresh-time" onload="autoRefreshTime()">20:49:37</span></div>
            <script>Date.prototype.format = function(fmt) {
                var o = {
                  "y+": this.getFullYear,
                  "M+": this.getMonth() + 1,
                  "d+": this.getDate(),
                  "h+": this.getHours(),
                  "m+": this.getMinutes(),
                  "s+": this.getSeconds()
                };
                if (/(y+)/.test(fmt)) fmt = fmt.replace(RegExp.$1, (this.getFullYear() + "").substr(4 - RegExp.$1.length));
                for (var k in o) if (new RegExp("(" + k + ")").test(fmt)) fmt = fmt.replace(RegExp.$1, (RegExp.$1.length == 1) ? (o[k]) : (("00" + o[k]).substr(("" + o[k]).length)));
                return fmt;
              }
              setInterval("document.getElementById('auto-refresh-date').innerHTML = (new Date()).format('yyyy年MM月dd日')", 1000);
              setInterval("document.getElementById('auto-refresh-time').innerHTML = (new Date()).format('hh:mm:ss')", 1000);</script>

                <div class="cut_line_1">
                </div>
            </div>
            <div class="guest_picture">
                <span id="jjl">
                    <img src="./图片/lsl.jpeg" alt="" width="135px">
                </span>
                <span id="green_line">
                    <img src="./图片/green_bg.gif" alt="" width="159px
                    ">
                </span>
            </div>
            <div class="guest_information">
                <ul>
                    <li>
                      <span class="w-title">姓名</span></li>
                    <li>
                      <span class="w-title">性别</span></li>
                    <li>
                      <span class="w-title">学工号</span></li>

                    <li>
                      <span class="w-title">学院</span></li>

                    <li>
                      <span class="w-title">辅导员</span></li>

                      <li>
                        <span class="w-title">辅导员电话</span></li>
                  </ul>
                  <table>
                    <tbody>
                        <tr>
                            <td>：</td>
                            <td>李世龙</td>
                        </tr>
                        <tr>
                            <td>：</td>
                            <td>男</td>
                        </tr>
                        <tr>
                            <td>：</td>
                            <td>18161803</td>
                        </tr>
                        <tr>
                            <td>：</td>
                            <td>飞行学院</td>
                        </tr>
                        <tr>
                            <td>：</td>
                            <td>黄焘</td>
                        </tr>
                        <tr>
                            <td>：</td>
                            <td>18698872301</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <div class="cut_line_2">
            </span>
            <div class="cut_line_2">
            </div>
            </div>
            <div class="pass_information">
                <p id="passport"><b>允许通行</b></p>
            </div>
        </div>
        <div class="box_bottom">
            <span id="bottom">
                <img src="./图片/WechatIMG3129.png" alt="" width="528px">
            </span>
        </div>
    </div>
    <script>

        function editinPut(e) {
            if (e===1){
                document.getElementById("enter_name").innerHTML='入校码';
            }else{
                document.getElementById("enter_name").innerHTML='出校码';
            }

        }

    </script>

    
    
</body>
</html>
