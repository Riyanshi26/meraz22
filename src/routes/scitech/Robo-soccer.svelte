<script>
    import Register from "./_Register.svelte";
</script>
<svelte:head>
	<title>Robo soccer | Meraz '22</title>
    <link href="https://fonts.googleapis.com/css2?family=Josefin+Sans&display=swap" rel="stylesheet">
</svelte:head>
<div class="bodyy">
    <div class="empty">

	</div>
    <div class="main-container">
        <div class="poster-container">
            <img alt="not found" class="poster1" src="/assets/poster/RoboSoccer.png"  border="0">
        </div>
        <div class="text-container">
            <div class="empty">

            </div>
            <div class="top-text">
                <h1 class="event-title">
                    ROBO SOCCER
                </h1>
                <Register link="https://forms.gle/snpeRiFfomRZ1Mc77"/>
                <h2 class="club-name">
                    EPSILON
                </h2>
            </div>
            <img alt="not found" class="top-design-class" src="/assets/top-design-use.png">
            <div class="description">
                <div class="description-container">
                    <p>Bring out The hidden Messi, Ronaldo in you and prove that ""No one plays soccer, better than engineers"". <br> The objective of this competition is to design a manual robot(wireless or wired) and which can compete in an arena designed for robotic soccer. Two robots will be placed in the arena, one bot will try to put ball in goal post and another bot will defend it.</p>
                </div>

                <div class="sub-container">
                    <div class="text">
                        <p>Event Mode- Offline</p>
                        <!-- <p>Registration Fee- Absolutely Free!</p> -->
                    </div>
                    <div class="button-container">
                        <a href="https://drive.google.com/file/d/1b1ihN_hiX4yNDDl10621kU0VUwMG5xsY/view?usp=drivesdk"><button class="glow-on-hover">Rulebook</button></a>
                    </div>
                </div>
            </div>
            <div class="details-container">
                <div class="prize-col">
                    <!-- <img alt="not found" src="event-template-assets/trophy-icon.png"> -->
                    <h3>Total Prize</h3>

                    &#8377;7,000 INR + Bluetooth Speaker <br>
                    &#8377;5,000 INR +  Neckband <br>
                    &#8377;3,000 INR  <br>
                    
                </div>
                <img alt="not found" class="breaker-design" src="/assets/breaker-design-use.png">
                <div class="poc-col">
                    <h3>Point Of Contact:</h3>

                    Mayank Chaturvedi: +91 8303354008 <br>
                    Kunal Singla: +91 7973203702 <br>
                    

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
		background-image: url('/assets/scitech_bg.png');
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
// height: 80vh;
// padding-top: 2%;
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
.event-title{
    display: flex;
}

@media screen and (max-width:900px){
    .event-title{
        padding-bottom: 10%;
    }
    .club-name{
        padding-bottom: 10%;
    }
.bodyy{
height: 250vh;
		// background-image: url(/assets/about_bg.png);
        // height: 170vh;
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
