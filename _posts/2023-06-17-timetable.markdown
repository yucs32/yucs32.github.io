---
layout : post
date:   2023-06-17 19:27:48 +0630
categories: timetabel
---
<html lang="en">
<head> 
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="icon" href="https://i.imgur.com/TJk9BEm.png" type="image/png">
    <title>Timetable</title>
    <style type="text/css">
.invisible {
  visibility: hidden;
}
.unselectable {
 -webkit-user-select: none; /* Safari */
 -moz-user-select: none; /* Firefox */
 -ms-user-select: none; /* IE10+/Edge */
 user-select: none; /* Standard */
}
table {
  margin: 0px;
}

.table-class td,
.table-class th {
  border: 1px solid grey;
  padding: 8px;
}


.winter-is-coming, .snow {
  z-index: 100;
  pointer-events: none;
}

.winter-is-coming {
  overflow: hidden;
  position: fixed;
  top: 0;
  height: 100%;
  width: 100%;
  max-width: 100%;
}

.snow {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  -webkit-animation: falling linear infinite both;
          animation: falling linear infinite both;
  -webkit-transform: translate3D(0, -100%, 0);
          transform: translate3D(0, -100%, 0);
}
.snow--near {
  -webkit-animation-duration: 10s;
          animation-duration: 10s;
  background-image: url("https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-large-075d267ecbc42e3564c8ed43516dd557.png");
  background-size: contain;
}
.snow--near + .snow--alt {
  -webkit-animation-delay: 5s;
          animation-delay: 5s;
}
.snow--mid {
  -webkit-animation-duration: 20s;
          animation-duration: 20s;
  background-image: url("https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-medium-0b8a5e0732315b68e1f54185be7a1ad9.png");
  background-size: contain;
}
.snow--mid + .snow--alt {
  -webkit-animation-delay: 10s;
          animation-delay: 10s;
}
.snow--far {
  -webkit-animation-duration: 30s;
          animation-duration: 30s;
  background-image: url("https://dl6rt3mwcjzxg.cloudfront.net/assets/snow/snow-small-1ecd03b1fce08c24e064ff8c0a72c519.png");
  background-size: contain;
}
.snow--far + .snow--alt {
  -webkit-animation-delay: 15s;
          animation-delay: 15s;
}

@-webkit-keyframes falling {
  0% {
    -webkit-transform: translate3D(-7.5%, -100%, 0);
            transform: translate3D(-7.5%, -100%, 0);
  }
  100% {
    -webkit-transform: translate3D(7.5%, 100%, 0);
            transform: translate3D(7.5%, 100%, 0);
  }
}

@keyframes falling {
  0% {
    -webkit-transform: translate3D(-7.5%, -100%, 0);
            transform: translate3D(-7.5%, -100%, 0);
  }
  100% {
    -webkit-transform: translate3D(7.5%, 100%, 0);
            transform: translate3D(7.5%, 100%, 0);
  }
}
    </style>
    <script type="text/javascript">
        function startTime()
        {
        var today=new Date();
        var h=today.getHours();
        var m=today.getMinutes();
        var s=today.getSeconds();
        m=checkTime(m);
        s=checkTime(s);
        document.getElementById('txt').innerHTML=h+":"+m+":"+s;
        t=setTimeout('startTime()',500);
        }
        function checkTime(i)
        {
        if (i<10)
        {
        i="0" + i;
        }
        return i;
        }
    </script>
</head>
<body bgcolor="skyblue" onload="startTime()" class="unselectable">
    <br>
    <h3 align="center">
        University of Yangon
        <br>
        2022-2023 Academic Year Time-Table
    </h3>
    <center>
      <table width="50%" border="0">
        <tr>
          <th align="left" colspan="2">
            Third Year, Second Semester
          </th>
        </tr>
        <tr>
          <th align="left">
            Computer Science Specification
          </th>
          <th align="right">
            <i id="txt"></i>
          </th>
        </tr>
      </table>
    </center>
    <br>
    <center>
        <table width="50%" height="250" border="3" class="table-class">
            <tr>
                <th rowspan="2">Day</th>
                <th align="center">&nbsp;9:00&nbsp;</th>
                <th align="center">10:00</th>
                <th align="center">11:00</th>
                <th align="center" rowspan="7">&nbsp;</th>
                <th align="center">12:30</th>
                <th align="center">13:30</th>
                <th align="center">14:30</th>
            </tr>
            <tr>
                <th>9:50</th>
                <th>10:50</th>
                <th>11:50</th>
                <th>13:20</th>
                <th>14:20</th>
                <th>15:20</th>
            </tr>
            <tr>
                <th align="center">Mon</th>
                <td align="center " colspan="2" title="Web-based System Development II">CS<i class="invisible">.</i>-<i class="invisible">.</i>3111</td>
                <td align="center" title="Computer Aided Software Enginerring">CS<i class="invisible">.</i>-<i class="invisible">.</i>3109</td>
                <td align="center" colspan="2" title="English">Eng<i class="invisible">.</i>-<i class="invisible">.</i>3001</td>
                <td align="center" title="Free Time">Machine</td>
            </tr>
            <tr>
                <th align="center">Tues</th>
                <td align="center " colspan="2" title="Software Process Management">CS<i class="invisible">.</i>-<i class="invisible">.</i>3108</td>
                <td align="center" title="Computer Aided Software Enginerring">CS<i class="invisible">.</i>-<i class="invisible">.</i>3109</td>
                <td align="center" colspan="2" title="Software Re-engineering">CS<i class="invisible">.</i>-<i class="invisible">.</i>3110</td>
                <td align="center" title="System Configuration Management">CS<i class="invisible">.</i>-<i class="invisible">.</i>3107</td>
            </tr>
            <tr>
                <th align="center">Wed</th>
                <td align="center " colspan="2" title="C#">CS<i class="invisible">.</i>-<i class="invisible">.</i>3108(C#)</td>
                <td align="center" title="System Configuration Management">CS<i class="invisible">.</i>-<i class="invisible">.</i>3107</td>
                <td align="center" colspan="2" title="Software Re-engineering">CS<i class="invisible">.</i>-<i class="invisible">.</i>3010</td>
                <td align="center" title="Computer Aided Software Enginerring">CS<i class="invisible">.</i>-<i class="invisible">.</i>3109</td>
            </tr>
            <tr>
                <th align="center">Thurs</th>
                <td align="center " colspan="2" title="English">Eng<i class="invisible">.</i>-<i class="invisible">.</i>3001</td>
                <td align="center" title="Web-based System Development II">CS<i class="invisible">.</i>-<i class="invisible">.</i>3111</td>
                <td align="center" colspan="2" title="System Configuration Management">Eng<i class="invisible">.</i>-<i class="invisible">.</i>3107</td>
                <td align="center" title="Software Re-engineering">CS<i class="invisible">.</i>-<i class="invisible">.</i>3110</td>
            </tr>
            <tr>
                <th align="center">Fri</th>
                <td align="center " colspan="2" title="Computer Aided Software Enginerring">CS<i class="invisible">.</i>-<i class="invisible">.</i>3109</td>
                <td align="center" title="Web-based System Development II">CS<i class="invisible">.</i>-<i class="invisible">.</i>3111</td>
                <td align="center" title="Free Time">Machine</td>
                <td align="center" title="Software Process Management">CS<i class="invisible">.</i>-<i class="invisible">.</i>3108</td>
                <td align="center" title="System Configuration Management">CS<i class="invisible">.</i>-<i class="invisible">.</i>3107</td>
            </tr>
        </table>
    </center>
    <p align="center">
        <font color="purple">
            <strong>
                ⬛U-208
            </strong>
        </font>
    </p>
    <div class="winter-is-coming">
        <div class="snow snow--near"></div>
        <div class="snow snow--near snow--alt"></div>
        
        <div class="snow snow--mid"></div>
        <div class="snow snow--mid snow--alt"></div>
        
        <div class="snow snow--far"></div>
        <div class="snow snow--far snow--alt"></div>
    </div>
</body>
</html>


