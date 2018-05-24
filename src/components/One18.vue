<template>
    <div>
        <main>
            <h1>{{ msg }}</h1>  
            <div class="wrapper">
                <div class="box sml a">
                    <img src="../assets/img/bar_1.jpg">
                </div>
                <div class="box smr b">
                    <h1>One18 Empire</h1>
                    <p>Located in vibrant Downtown Calgary, ONE18 Empire is a whisk(e)y-inspired bar and restaurant with a strong focus on sharable, locally inspired cuisine, masterfully paired with our select onsite reserve.</p>
                </div>
                <div class="box c">
                    <div class="box c0">
                        <h2>Highlights</h2>
                    </div>
                    <div class="box c1">
                        <h4>Ardbeg Vintage 1977</h4>
                        <p>Distillery Bottling</p>
                        <h4>Bowmore 30 years Sea Dragon</h4>
                        <p>Distillery Bottling, late 1990s</p>
                        <h4>Macallan 32 years 1973</h4>
                        <p>Gordon & Macphail, Vintage Speymatt</p>
                    </div>
                </div>
                <div class="box d">
                    <div class="box d0">
                        <h2>Opening hours</h2>
                    </div>
                    <div class="box d1">
                        <h3>Mon - Fri</h3>
                        <h3>Sat - Sun</h3>
                    </div>
                    <div class="box d2">
                        <h3>6.30am to late</h3>
                        <h3>7am to late</h3>
                    </div>
                    <div class="box d3">
                        <h2>Happy Hour</h2>
                        <h3>Every day till 6pm</h3>
                    </div>
                </div>
                <div class="box lgm e">
                    <h2>Specials</h2>
                </div>
                <div class="box sml f">
                    <img src="../assets/img/ardbeg_tasting.jpg">
                </div>
                <div class="box smr g">
                    <h3>Ardbeg Event: Peat & Love
                            <span>May 17, 2018</span>
                    </h3>
                    <p>For over 200 years, Ardbeg has been made on the small, remote Scottish Isle of Islay. Some people trael to Ardbeg along the winding road form Port Ellen. Others follow their nose, their destiny or the advice of a good friend.</p>
                </div>
                <div class="box sml h">
                    <img src="../assets/img/tasting.png">
                </div>
                <div class="box smr i">
                    <h3>Discovery tasting: Scotland
                        <span>Jun 14, 2018</span>
                    </h3>
                    <p>We're offering a brand new premium tasting experience, fascinating for anyone interested in Scotland and its rich distilling heritage.</p>
                </div>
                <div class="box lgm j">
                    <h2>How to find us</h2>
                </div>
                <div class="box sml k">
                    <h3>820 Centre Street SE Calgary, Alberta<br />
                        <br />
                        info@one18empire.com<br />
                        <br />
                        403.269.0299
                    </h3>
                </div>
                <div class="box smr l">
                    <img src="../assets/img/map2.png">
                </div>
            </div>
        </main>
    </div>
</template>

<script>
export default {
    name: 'One18',
    props: {
        msg: String
    }
}
</script>
        
<style scoped>
* {
    box-sizing: border-box;
}
    body {
    border: 1px solid black;
    width: 95%;
    margin: auto;
    font-family: 'Architects Daughter', cursive;
    }
    .wrapper {
            display: flex;
            flex-flow: row wrap;
            padding: 4vw;
        }
        .box {
            /* border: 1px solid black; */
            padding: 1vw;
            flex: 50 1 50%;
        }
        .sml {
            flex: 40 1 40%;
        }
        .lgm {
            flex: 100 1 100%;
        }
        img {
            width: auto;
        }

        .b {
            padding-left: 4vw;
        }
        .c1, .d1, .d2 {
            line-height: 0vw;
        }
        .d {
            display: grid;
            grid-template-columns: 1fr 1fr;
        }
        .d0, .d3 {
            grid-column: 1 / span 2;
            text-align: center;
        }
        .d1 {
            grid-column: 1;
            text-align: left;
        }
        .d2 {
            grid-column: 2;
            text-align: right;
        }

        img {
            width: 100%;
        }
        h1 {
            font-size: 4.5vw;
            margin: 0.25vw;
        }
        h2 {
            font-size: 2.5vw;
            margin: 0.1vw;
            text-align: center;
        }
        h3 {
            font-size: 2vw;
        }
        h4 {
            font-size: 2vw;
        }
        p {
            font-size: 1.6vw;
        }


        
        @media screen and (max-width: 700px) {
            .box {   
                flex-direction: column;
                flex: 1 1 100%;
            }
        }
</style>

