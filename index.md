<!DOCTYPE html>
<html lang="en" style="font-family:'未曾忘记那位少年';">
    <head>
        <meta charset="utf-8">
        <title>Dy Audio Processor</title>
    </head>
    <style>
        @font-face
        {
            font-family: 未曾忘记那位少年;
            src: url("fonts/font.ttf");
        }

        div
        {
            font-family: 未曾忘记那位少年;
        }
    </style>
    <div>
        <img src="img\Duyu_Logo.jpg" width="120" height="120" id="img001">
    </div>
    <style>
        #img001
        {
            position:absolute;
            left:1.5%;
            top: 2%;
            z-index:9999;
            border-radius: 15%;
        }
    </style>
    <style>
        @font-face
        {
            font-family:font001;
            src: url(fonts/font.ttf);
        }
    </style>
    <div id="div001">
        <font face="未曾忘记那位少年" size="5" color="white">
            <p><h1 style="text-align:center">Download Duyu Audio Processor</h1></p>
        </font>
    </div>
    <div id="div002">
    </div>
    <div id="div003">
        <font face="未曾忘记那位少年" size="2" color="white">
            <p><h1 style="text-align:center">Copyright (c) 2022 Qilu University of Technology - Duyu.</h1></p>
            <p><h1 style="text-align:center">All Rights Reserved.</h1></p>
        </font>
    </div>
    <style>
        #div001
        {
            position: absolute;
            left:0%;
            top: 0%;
            width:100%;
            height:25%;
            background: rgb(0, 0, 0);
        }
        #div003
        {
            position: absolute;
            left:0%;
            top: 165%;
            width:100%;
            height:20%;
            background: rgb(0, 0, 0);
        }
        #div002
        {
            position: absolute;
            left:0%;
            top: 25%;
            width:100%;
            height:160%;
            background: rgb(34, 34, 34);
        }
    </style>
    <div id="div004">
        <font face="未曾忘记那位少年" size="3" color="white">
            <p><h1>
                <em>Experience Vocal-Cut Moudle of Duyu Audio Processor</em>
            </h1></p>
        </font>
    </div>
    <div id="div007">
        <div id="div008">
            <font face="未曾忘记那位少年" size="3" color="white">
                <p><h1>
                    1.Original Sound
                </h1></p>
            </font>
        </div>
        <audio src="audio\01.mp3" autoplay="false" controls="true" id="audio001" ontimeupdate="updata01()"></audio>
    </div>
    <div id="div009">
        <div id="div010">
            <font face="未曾忘记那位少年" size="3" color="white">
                <p><h1>
                    2.Using Channel-Mix Algorithm
                </h1></p>
            </font>
        </div>
        <audio src="audio\02.mp3" autoplay="false" controls="true" id="audio002" ontimeupdate="updata02()"></audio>
    </div>
    <div id="div011">
        <div id="div012">
            <font face="未曾忘记那位少年" size="3" color="white">
                <p><h1>
                    3.Machine-Learning Algorithm
                </h1></p>
            </font>
        </div>
        <audio src="audio\03.mp3" autoplay="false" controls="true" id="audio003" ontimeupdate="updata03()"></audio>
    </div>
    <div id="div013">
        <div id="div014">
            <font face="未曾忘记那位少年" size="3" color="white">
                <p><h1>
                    4.Standard Accompaniment
                </h1></p>
            </font>
        </div>
        <audio src="audio\04.mp3" autoplay="false" controls="true" id="audio004" ontimeupdate="updata04()"></audio>
    </div>
    <script>
        var x001 = document.getElementById("audio001");
        var x002 = document.getElementById("audio002");
        var x003 = document.getElementById("audio003");
        var x004 = document.getElementById("audio004");
        window.ctime = 0;
        function setHalfVolume()
        {
            x001.volume = 0.75;
            x002.volume = 0.75;
            x003.volume = 0.75;
            x004.volume = 0.75;
        }
        window.onload=function()
        {
            setHalfVolume();
        }
        x001.onplay=function()
        {
            x002.pause();
            x003.pause();
            x004.pause();
            x001.currentTime=window.ctime;
        }
        x002.onplay=function()
        {
            x001.pause();
            x003.pause();
            x004.pause();
            x002.currentTime=window.ctime;
        }
        x003.onplay=function()
        {
            x001.pause();
            x002.pause();
            x004.pause();
            x003.currentTime=window.ctime;
        }
        x004.onplay=function()
        {
            x001.pause();
            x002.pause();
            x003.pause();
            x004.currentTime=window.ctime;
        }
        updata01=function ()
        {
            window.ctime=x001.currentTime;
        }
        updata02=function ()
        {
            window.ctime=x002.currentTime;
        }
        updata03=function ()
        {
            window.ctime=x003.currentTime;
        }
        updata04=function ()
        {
            window.ctime=x004.currentTime;
        }


    </script>
    <div id="div005">
        <img src="img\Album_Poster.jpg" width="160" height="160" id="img002">
    </div>
    <div id="div006">
        <font face="未曾忘记那位少年" size="1" color="white">
            <p><h1>
                Timi Zhuo - Dull Ice Flower<br>
                Television Golden Grand Hits<br>
                Released in 1998.
            </h1></p>
        </font>
    </div>
    <style>
        #audio001
        {
            position: absolute;
            left: 50%;
            top: 33%;
            width: 30%;
            color:rgb(255, 255, 255);
        }
        #audio002
        {
            position: absolute;
            left: 50%;
            top: 45%;
            width: 30%;
            color:rgb(255, 255, 255);
        }
        #audio003
        {
            position: absolute;
            left: 50%;
            top: 57%;
            width: 30%;
            color:rgb(255, 255, 255);
        }
        #div010
        {
            position: absolute;
            left:20%;
            top:42%;
        }
        #div004
        {
            position: absolute;
            left:1.5%;
            top:22%;
        }
        #div006
        {
            position: absolute;
            left:1.5%;
            top:61%;
        }
        #img002
        {
            position:absolute;
            left:3%;
            top: 35%;
            z-index:9999;
            border-radius: 7%;
        }
        #div008
        {
            position: absolute;
            left:20%;
            top:31.5%;
        }
        #div012
        {
            position: absolute;
            left:20%;
            top:54%;
        }
        #div014
        {
            position: absolute;
            left:20%;
            top:65%;
        }
        #audio004
        {
            position: absolute;
            left: 50%;
            top: 69%;
            width: 30%;
            color:rgb(255, 255, 255);
        }
    </style>
    <div id="div015">
        <font face="未曾忘记那位少年" size="1.5" color="white">
            <p><h1>
                The algorithm of channel-mix was made by Python.We used library of Numpy to edit wave of sound.
                For Multi-channel audio,the sound of person is always the same in different channels,
                but the sound of music instruments is not same.So according to this facts,I used Python
                to subtract the same part of the two waves,and the left thing is accompaniment.
                The algorithm of Machine-Learning is based on Tenserflow,which is an AI library for python.But here,
                I get a version written in C++ on GitHub,so I used that.It is better to use AI algorithm,because it is 
                high-technology.And fortunatlly,this software is not only source-open but also free!
            </h1></p>
        </font>
    </div>
    <div id="div016">
        <font face="未曾忘记那位少年" size="3" color="white">
            <p><h1 style="text-align:center">
                The Reasons Why You Should Choose DY Audio Processor....
            </h1></p></em>
        </font>
    </div>
    <style>
        #div015
        {
            position: absolute;
            left: 1.5%;
            top: 98%;
            width: 40%;
        }
        #div016
        {
            position: absolute;
            left: 0%;
            top: 83%;
            width: 100%;
            background: rgb(0, 0, 0);
            height: 11%;
        }
    </style>

    <div id="div017">
        <a href="src\DyAudioProcessor.exe"><img src="img\Download.jpg" id="img003"></a>
    </div>
    <img src="img\codes.jpg" id="img004">
    <style>
        #img003
        {
            position: absolute;
            left:82%;
            top:13%;
            width:15%;
            height: 10%;
            z-index: 99999;
            border-radius: 10%;
        }
        #img004
        {
            position: absolute;
            left:43%;
            width: 56%;
            top:97%;
            height: 65%;
            border-radius: 15%;
        }
    </style>
    <div id="div018">
        <font face="未曾忘记那位少年" size="0.5" color="white">
            <p><h1 style="text-align:center">
                Source Code of this Project Location:<br>
                <a href="http://github.com/duyu09/">http://github.com/duyu09/</a>
            </h1></p>
        </font>
    </div>
    <img id="img005" src="img\Quality.jpg">
    <style>
        #div018
        {
            position: absolute;
            top:147%;
            left:10%;
        }
        #img005
        {
            position: absolute;
            top:30%;
            left:82%;
            width: 7%;
            border-radius: 20%;
        }
    </style>
    <hidden>
        Copyright (c) 2022 Qilu University of Technology - Duyu.<br>
        All Rights Reserved.
    </hidden>
</html>
