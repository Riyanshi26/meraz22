<svelte:head>
	<title> Breaking Barriers 2.0 | Meraz '22</title>
    <link href="https://fonts.googleapis.com/css2?family=Josefin+Sans&display=swap" rel="stylesheet">
</svelte:head>
<div class="bodyy">
    	<div class="empty">

	</div>
    <div class="main-container">
        <div class="poster-container">
            <img alt="not found" class="poster1" src="/assets/poster/Breaking Barriers 2.0.png"  border="0">
        </div>
        
        <div class="text-container">
            <div class="empty">

            </div>
            <div class="top-text">
                <h1 class="event-title">
                    BREAKING BARRIERS 2.0
                </h1>
                <h2 class="club-name">
                    NIRVANA
                </h2>
            </div>
            <img alt="not found" class="top-design-class" src="/assets/top-design-use.png">
            <div class="description">
                <div class="description-container">
            
                    <p>This event promote aesthetics that are gender non-
conforming to break the gender barriers. We will be keeping multiple booths where we focus on what are
perceived as feminine aesthetics. This event aims at casting out toxic masculinity and few gender related
stereotypes.
So gear up for Breaking Barriers 2.0 and get your nails, eye makeup or mehndi done while having (or not
having) a nice chat about gender and sexuality!
                    
                </div>

                <div class="sub-container">
                    <div class="text">
                        <p>Event Mode- Offline</p>
                        <!-- <p>Registration Fee- Absolutely Free!</p> -->
                    </div>
                    <div class="button-container">
                        <a href="https://drive.google.com/drive/folders/1CVUx279l1zaXV5w9PfVAHn5N03HiQ3sW?usp=sharing">
                        <button class="glow-on-hover">Rulebook</button></a>
                    </div>
                </div>
            </div>
            <div class="details-container">
                <div class="prize-col">
                     

                     <!-- <img alt="not found" src="event-template-assets/trophy-icon.png"> -->

                    
                </div>
                <img alt="not found" class="breaker-design" src="/assets/breaker-design-use.png">
                <div class="poc-col">
                    <h3>Point Of Contact:</h3>

                    Santaz Sahithi : +91 95734 24443 <br>
                    Srilekha Kadambala : +91 93900 99543<br>
                    Sri Koumudi : +91 89195 59221<br>

                </div>
            </div>
            <img alt="not found" src="/assets/bottom-design-use.png">
        </div>
    </div>
</div>

<style lang="scss">
	* {
		margin: 0;
		padding: 0;
	}

	.bodyy {
		/* background-color: black; */
		background-image: url('/assets/info_bg.png');
		color: white;
		padding-top: 5vw;
height: 120vh;
        background-size: cover;
        background-repeat: no-repeat;
		font-family: 'Josefin Sans', sans-serif;
	}
	.main-container{
    display:flex;
    margin-left:6%;
    margin-right:6%;
    object-fit:contain;
    flex-grow: 1;
    height:60vw;
}

.poster-container{
flex-basis:70%;
padding-top: 3%;
/* flex-grow: 1; */
}

.poster1{
    width:100%;
    height:auto;
    border:2px solid teal;
    border-radius: 2px;
}
.text-container{
    padding:2% 3%;
    /* flex-grow:3; */
}

.event-title{
    font-size: 5vh;
    padding-left:1vw;
}

.club-name{
    font-size:3.3vh;
    padding-top:0.5vw;
    font-family: 'Josefin Sans', sans-serif;
    padding-left:1vw;
}

img{
    max-width: 100%;
}

.top-design-class{
    margin-top: 1vw;
}

.description{
    padding-left:0.8vw;
    padding-right:0.8vw;
    min-height: 10vw;
    font-family: 'Josefin Sans', sans-serif;
}

.description-container p{
    line-height: 25px;
    margin-top:2vw;
    /* font-size: 1.1vw; */
}

.sub-container{
    display:grid;
    grid-template-columns: 50% 50%;
    margin-top:3vw;
}

.text{
    display:flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    align-content: center;
}

.button-container{
    display: inline-flex;
    justify-content: center;
    align-content: center;
    flex-direction: column;
    padding-left: 20%;
}

/* ----------------- button animation begins ---------------------- */

.glow-on-hover {
    width: 10vw;
    height: 2vw;
    border: none;
    outline: none;
    color: #fff;
    background: #111;
    cursor: pointer;
    position: relative;
    z-index: 0;
    border-radius: 10px;
}

.glow-on-hover:before {
    content: '';
    background: linear-gradient(45deg, #ff0000, #ff7300, #fffb00, #48ff00, #00ffd5, #002bff, #7a00ff, #ff00c8, #ff0000);
    position: absolute;
    top: -2px;
    left:-2px;
    background-size: 400%;
    z-index: -1;
    filter: blur(5px);
    width: calc(100% + 4px);
    height: calc(100% + 4px);
    animation: glowing 20s linear infinite;
    opacity: 0;
    transition: opacity .3s ease-in-out;
    border-radius: 10px;
}

.glow-on-hover:active {
    color: #000
}

.glow-on-hover:active:after {
    background: transparent;
}

.glow-on-hover:hover:before {
    opacity: 1;
}

.glow-on-hover:after {
    z-index: -1;
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    background: #111;
    left: 0;
    top: 0;
    border-radius: 10px;
}

@keyframes glowing {
    0% { background-position: 0 0; }
    50% { background-position: 400% 0; }
    100% { background-position: 0 0; }
}

/* ----------------- button animation ends ---------------------- */
.event-title{
    display: flex;
}
.details-container{
    padding:2.2vw;
    display:grid;
    grid-template-columns: 45% 10% 45%;
    line-height:25px;
}

.breaker-design{
    height:17vh;
    width:auto;
}

.prize-col{
    text-align: center;
    display: flex;
    justify-content: center;
    align-content: center;
    flex-direction: column;
}

.prize-col img{
    display:inline;
}

.poc-col{
    display: flex;
    justify-content: center;
    align-content: center;
    flex-direction: column;
    text-align:center;
}


@media screen and (max-width:900px){
.bodyy{
height: 250vh;
		// background-image: url(/assets/about_bg.png);
        // height: 150vh;
		background-attachment: fixed;
		background-size: cover;
		background-repeat:no-repeat ;
	}
	.empty {
		height: 80px;
	}

   .main-container{
    flex-direction:column;
   }

   .details-container{
    margin-top:3vh;
   }

.button-container{
    padding-left: 30%;
}

   .glow-on-hover{
    min-width:17vw;
    min-height:2.3vh;
   }
}
</style>
