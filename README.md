# animated-mining-screen
<style>
        body {
            background-color: #272727;
        }

        .fakeButtons {
            height: 10px;
            width: 10px;
            border-radius: 50%;
            border: 1px solid #000;
            position: relative;
            top: 6px;
            left: 6px;
            background-color: #ff3b47;
            border-color: #9d252b;
            display: inline-block;
        }

        .fakeMinimize {
            left: 11px;
            background-color: #ffc100;
            border-color: #9d802c;
        }

        .fakeZoom {
            left: 16px;
            background-color: #00d742;
            border-color: #049931;
        }

        .fakeMenu {
            width: 650px;
            box-sizing: border-box;
            height: 25px;
            background-color: #bbb;
            margin: 0 auto;
            border-top-right-radius: 5px;
            border-top-left-radius: 5px;
        }

        .fakeScreen {
            background-color: #151515;
            box-sizing: border-box;
            width: 650px;
            height: 400px;
            margin: 0 auto;
            padding: 20px;
            border-bottom-left-radius: 5px;
            border-bottom-right-radius: 5px;
        }

        .fakeScreen p {
            position: relative;
            text-align: left;
            font-size: 1.25em;
            font-family: consolas;
            white-space: nowrap;
            overflow: hidden;
            width: 0;
        }

        .fakeScreen span {
            color: #fff;
            font-weight: bold;
        }

        .line1 {
            color: #9CD9F0;
            -webkit-animation: type 0.5s 1s steps(20, end) forwards;
            -moz-animation: type 0.5s 1s steps(20, end) forwards;
            -o-animation: type 0.5s 1s steps(20, end) forwards;
            animation: type 0.5s 1s steps(20, end) forwards;
        }

        .cursor1 {
            -webkit-animation: blink 1s 2s 2 forwards;
            -moz-animation: blink 1s 2s 2 forwards;
            -o-animation: blink 1s 2s 2 forwards;
            animation: blink 1s 2s 2 forwards;
        }

        .line2 {
            color: #CDEE69;
            -webkit-animation: type 0.5s 4.25s steps(20, end) forwards;
            -moz-animation: type 0.5s 4.25s steps(20, end) forwards;
            -o-animation: type 0.5s 4.25s steps(20, end) forwards;
            animation: type 0.5s 4.25s steps(20, end) forwards;
        }

        .cursor2 {
            -webkit-animation: blink 1s 5.25s 2 forwards;
            -moz-animation: blink 1s 5.25s 2 forwards;
            -o-animation: blink 1s 5.25s 2 forwards;
            animation: blink 1s 5.25s 2 forwards;
        }

        .line3 {
            color: #E09690;
            -webkit-animation: type 0.5s 7.5s steps(20, end) forwards;
            -moz-animation: type 0.5s 7.5s steps(20, end) forwards;
            -o-animation: type 0.5s 7.5s steps(20, end) forwards;
            animation: type 0.5s 7.5s steps(20, end) forwards;
        }

        .cursor3 {
            -webkit-animation: blink 1s 8.5s 2 forwards;
            -moz-animation: blink 1s 8.5s 2 forwards;
            -o-animation: blink 1s 8.5s 2 forwards;
            animation: blink 1s 8.5s 2 forwards;
        }

        .endline {
            color: #fff;
            -webkit-animation: type 0.5s 10.75s steps(20, end) forwards;
            -moz-animation: type 0.5s 10.75s steps(20, end) forwards;
            -o-animation: type 0.5s 10.75s steps(20, end) forwards;
            animation: type 0.5s 10.75s steps(20, end) forwards;
        }

        .endcursor {
            -webkit-animation: blink 1s 11.5s infinite;
            -moz-animation: blink 1s 8.5s infinite;
            -o-animation: blink 1s 8.5s infinite;
            animation: blink 1s 8.5s infinite;
        }

        @-webkit-keyframes blink {
            0% {
                opacity: 0;
            }
            40% {
                opacity: 0;
            }
            50% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                opacity: 0;
            }
        }

        @-moz-keyframes blink {
            0% {
                opacity: 0;
            }
            40% {
                opacity: 0;
            }
            50% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                opacity: 0;
            }
        }

        @-o-keyframes blink {
            0% {
                opacity: 0;
            }
            40% {
                opacity: 0;
            }
            50% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                opacity: 0;
            }
        }

        @keyframes blink {
            0% {
                opacity: 0;
            }
            40% {
                opacity: 0;
            }
            50% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                opacity: 0;
            }
        }

        @-webkit-keyframes type {
            to {
                width: 17em;
            }
        }

        @-moz-keyframes type {
            to {
                width: 17em;
            }
        }

        @-o-keyframes type {
            to {
                width: 17em;
            }
        }

        @keyframes type {
            to {
                width: 17em;
            }
        }
    </style>
    <div class="fakeMenu">
        <div class="fakeButtons fakeClose"></div>
        <div class="fakeButtons fakeMinimize"></div>
        <div class="fakeButtons fakeZoom"></div>
    </div>
    <div class="fakeScreen">
        <p class="line1">&#062; mining started<span class="cursor1">_</span></p>
        <p class="line2">&#062; mining on miner-sim.com:4004 pool<span class="cursor2">_</span></p>
        <p class="line3">&#062; block found - mining it!<span class="cursor3">_</span></p>
        <p class="endline">><span class="endcursor">_</span></p>
    </div>