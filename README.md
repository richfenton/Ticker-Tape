# Ticker-Tape
Sets top of page ticker tape message within portal 

<body>
    <div class="tcontainer">
        <div class="ticker-wrap">
            <div class="ticker-move">
                <div class="ticker-item">{{Forename}} By Making The Minimum Payment of £{{min_due}} You May Be Able To Freeze Interest on Your Account.</div>
								<div class="ticker-item">{{Forename}} By Making The Minimum Payment of £{{min_due}} You May Be Able To Freeze Interest on Your Account.</div>
								<div class="ticker-item">{{Forename}} By Making The Minimum Payment of £{{min_due}} You May Be Able To Freeze Interest on Your Account.</div>
								<div class="ticker-item">{{Forename}} By Making The Minimum Payment of £{{min_due}} You May Be Able To Freeze Interest on Your Account.</div>
            </div>
        </div>
    </div>
  
   .ticker-wrap {
        width: 100%;
        padding-left: 100%;
        background-color: none;
    }
    
    @keyframes ticker {
        100% {
            transform: translate3d(-100%, 0, 0);
        }
    }
    
    .ticker-move {
        display: inline-block;
        white-space: nowrap;
        padding-right: 100%;
        animation-timing-function: linear;
        animation: ticker 40s linear infinite;
    }
    
    .ticker-move:hover {
        animation-play-state: running;
    }
    
    .ticker-item {
        display: inline-block;
        padding: 0 40px;
        font-size: 25px;
        font-weight: bold;
        color: #0076C1 !important;
    }
