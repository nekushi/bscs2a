<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>BSCS-2A</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
        html {
            scroll-behavior: smooth;
        }
        body {
            width: 100%;
            height: auto;
            padding: 5%;
            margin: 0;
            box-sizing: border-box;
            background: #ddd;
            display: flex;
            flex-flow: column wrap;
            gap: 20px;
        }
        .top-holder {
            position: fixed;
            left: 50%;
            transform: translate(-50%, 0);
        }
        .logo-and-friends {
            display: flex;
            justify-content: space-around;
        }
        .head {
            width: 35%;
            aspect-ratio: 1 / 1;
        }
        .ham {
            position: relative;
            width: 100%;
            height: 25px;
        }
        .borgar, #toggler {
            position: absolute;
            left: 50%;
            transform: translate(-50%, 0);
            display: flex;
            justify-content: space-between;
            flex-flow: column nowrap;
            height: 100%;
        }
        #toggler {
            outline: none;
            visibility: hidden;
            height: 25px;
            width: 25px;
            left: 37%;
        }
        .line {
            background: black;
            border-radius: 10px;
            width: 30px;
            height: 5px;
            transition: all 300ms ease;
        }
        .nav {
            height: 60px;
            width: 100%;
            display: flex;
            justify-content: space-evenly;
            align-items: flex-end;
        }
        .a {
            color: #000;
            visibility: hidden;
            padding: 0 20px;
            border-radius: 10px;
            text-decoration: none;
            outline: none;
            background: linear-gradient(to right, #0057ff, #0057ff);
            background-size: 0% 2px;
            background-repeat: no-repeat;
            background-position: center bottom;
            transition: background 300ms ease;
        }
        .a:hover {
            background-size: 65% 2px;
        }
        .asible {
            visibility: visible;
        }
        .one1 {
            transform-origin: left;
            transform: rotate(42deg);
            transition: transform 300ms ease;
        }
        .two2 { 
            display: none;
            transition: display 300ms ease;
        } 
        .three3 {
            transform-origin: left;
            transform: rotate(-42deg);
            transition: transform 300ms ease;
        } 
        #info, #officers, #students, #others {
            padding: 5%;
            background: #4077ff;
            border-radius: 20px;
            margin-top: 20px;
        }
        .info {
            text-indent: 40px;
            text-align: justify;
        }
        .school {
            display: inline-block;
            width: 49%;
            aspect-ratio: 1 / 1;
            border-radius: 15px;
        }
        .officer-container {
            display: flex;
            align-items: center;
            justify-content: space-evenly;
            flex-flow: column nowrap;
        } 
        .off {
            border-radius: 100%;
            width: 30%;
            aspect-ratio: 1 / 1;
            display: block;
        }
        .off-handler {
            display: flex;
            justify-content: space-evenly;
            align-items: center;
            flex-flow: column wrap;
            text-align: center;
        }
        span {
            font-weight: 700;
        }
        .misc {
            padding-left: 10px;
        }
        .misc {
            position: relative;
            display: flex;
            flex-flow: column wrap;
            align-items: baseline;
        }
        .misc::before {
            content: "";
            position: absolute;
            top: 0;
            left: -10px;
            height: 110px;
            width: 5px;
            background: #b9735d;
            margin: 0 10px;
            border-radius: 5px;
        }
        i {
            font-size: 22px;
        }
        .dev {
            margin-top: 15px;
        }
        .smol {
            display: block;
            font-size: 5px;
        }
        .bahala-na {
            scroll-behavior: smooth;
            margin-top: 180px;
            height: 500px;
            overflow: auto;
            scroll-snap-type: y mandatory;
        }
    </style>
</head>
<body>
    <div class="top-holder">
    <div class="logo-and-friends">
        <img src="ti.png" class="head logo" />
        <img src="bscs.png" class="head course" />
    </div>
    <div class="ham">
        <div class="borgar">
        <div class="line one"></div>
        <div class="line two"></div>
        <div class="line three"></div>
    </div>
    <div class="nav">
        <a href="#info" class="a">Info</a>
        <a href="#officers" class="a">Officers</a>
        <a href="#students" class="a">Students</a>
        <a href="#others" class="a">Others</a>
    </div>
    </div>
    </div>
    
    <div class="bahala-na">
    <div id="info">
        <h2>INFO</h2>
        <p class="info">
            Tanauan Institute (TI), Inc. is a private higher educational institution in Batangas. It is owned by the Collantes Family and located at J. Gonzales, Barangay 4, Tanauan City Batangas.
        </p>
        <p class="info">
            This private school offer Elementary, Junior High School, Senior High School and College Education.
        </p>

        <div class="mission">
            <h3>• Mission</h3>
            <p class="info">
                Tanauan Institute, Inc. seeks to establish a culture of intellectual competence, environmental awareness and socio civic responsibility. Tanauan Institute, Inc. commits itself to the formation of disciplined and enlightened minds. Tanauan Institute, Inc. aims to help build a nation of great men and women who shall be accomplished and decorated in their fields.
            </p>
        </div>
        <div class="Vision">
            <h3>• Vision</h3>
            <p class="info">
                Tanauan Institute, Inc. envision itself to be a world class institution dedicated to the higher learning and modern research. It hopes to contribute to the humane and holistic development of the Filipino youth through top tier quality education. Tanauan Institute, Inc. strives to produce socially and morally upright individual in globally competitive environment.
            </p>
        </div>
        <div class="preamble">
            <h3>• Preamble</h3>
            <p class="info">
                We, the sovereign Filipino people, imploring the aid of Almighty God, in order to build a just and humane society, and establish a Government that shall embody our ideals and aspirations, promote the common good, conserve and develop our patrimony, and secure to ourselves and our posterity, the blessings of independence and democracy under the rule of law and a regime of truth, justice, freedom, love, equality, and peace, do ordain and promulgate this Constitution.
            </p>
        </div>
        <img src="one.jpeg" class="school ti1" />
        <img src="two.jpeg" class="school ti2" /> 
    </div>
    
    <div id="officers">
        <h2 class="heading-officers">BSCS-2A OFFICERS</h2>
        <div class="officer-container">
            <div class="off-handler">
                <img src="https://scontent.fmnl24-1.fna.fbcdn.net/v/t39.30808-1/371070779_1382535555636230_8959667858757645950_n.jpg?stp=c0.5000x0.5000f_dst-webp_e15_p258x258_q70_tt1_u&efg=eyJ1cmxnZW4iOiJ1cmxnZW5fZnJvbV91cmwifQ&_nc_eui2=AeFi7isw9mtMWVZkRAI2PAezTugHWaD0OR9O6AdZoPQ5H3DZO9Wqg19HzG5FdF5kZGrMrNug9I1e69X90U0wNi6M&_nc_cid=0&_nc_ad=z-m&_nc_rml=0&_nc_ht=scontent.fmnl24-1.fna&_nc_cat=101&_nc_ohc=vsxh9KU3DTkAX-yJ8uC&ccb=1-7&_nc_sid=5fac6f&oh=00_AfBMu_Po21oseQEje-zyTpXGVZDS_zvTOlBNHhSOJ8bTvA&oe=6511D850" class="off president"/>
                <p><span>Bernadette Ramos</span><br />President</p>
            </div>
            <div class="off-handler">
                <img src="https://scontent.fmnl24-1.fna.fbcdn.net/v/t39.30808-1/378294530_2959843730815380_7805518303662697696_n.jpg?stp=c0.5000x0.5000f_dst-webp_e15_p258x258_q70_tt1_u&efg=eyJ1cmxnZW4iOiJ1cmxnZW5fZnJvbV91cmwifQ&_nc_eui2=AeFli6vweazm2E2495Vv03zX6ogVyK9ygXvqiBXIr3KBe5-G3sJgNTqbJh-lClYTOmqQrvOwgh1GbiqlMj5UI3ft&_nc_cid=0&_nc_ad=z-m&_nc_rml=0&_nc_ht=scontent.fmnl24-1.fna&_nc_cat=107&_nc_ohc=imYb5Kl0upgAX_AiOQ5&ccb=1-7&_nc_sid=5fac6f&oh=00_AfBOksDO2zG-rcPr6QqV-M_zBr1eY8BcZRKAjNbHobZ52w&oe=6511577B" class="off vice-president"/>
                <p><span>Lorenz De Vera</span><br />Vice President</p>
            </div>
            <div class="off-handler">
                <img src="https://scontent.fmnl24-1.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=c0.5000x0.5000f_dst-webp_e15_p258x258_q70_tt1_u&efg=eyJ1cmxnZW4iOiJ1cmxnZW5fZnJvbV91cmwifQ&_nc_eui2=AeFc3UC6mD55ly-YrK3kzvuEso2H55p0AlGyjYfnmnQCUcXIT08tIAPXGs2far4vOLSGAFaeS7XY4Bvc9K_AU4GB&_nc_cid=0&_nc_ad=z-m&_nc_rml=0&_nc_ht=scontent.fmnl24-1.fna&_nc_cat=1&_nc_ohc=OlcdNEVMsJMAX_SxXN7&ccb=1-7&_nc_sid=dbb9e7&oh=00_AfDTed6I-CRC6gNpHL7DqwUnc0cerUXO8WXQbKhcdSWpHg&oe=652E6838" class="off secretary"/>
                <p><span>Kristel Anne Sarmiento</span><br />Secretary</p>
            </div>
            <div class="off-handler">
                <img src="https://scontent.fmnl24-1.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=c0.5000x0.5000f_dst-webp_e15_p258x258_q70_tt1_u&efg=eyJ1cmxnZW4iOiJ1cmxnZW5fZnJvbV91cmwifQ&_nc_eui2=AeFc3UC6mD55ly-YrK3kzvuEso2H55p0AlGyjYfnmnQCUcXIT08tIAPXGs2far4vOLSGAFaeS7XY4Bvc9K_AU4GB&_nc_cid=0&_nc_ad=z-m&_nc_rml=0&_nc_ht=scontent.fmnl24-1.fna&_nc_cat=1&_nc_ohc=OlcdNEVMsJMAX_SxXN7&ccb=1-7&_nc_sid=dbb9e7&oh=00_AfDTed6I-CRC6gNpHL7DqwUnc0cerUXO8WXQbKhcdSWpHg&oe=652E6838" class="off president"/>
                <p><span>Kriztel Anne Solis</span><br />Treasurer</p>
            </div>
            <div class="off-handler">
                <img src="https://scontent.fmnl24-1.fna.fbcdn.net/v/t39.30808-1/372845247_1592931197904298_8824517834455952245_n.jpg?stp=c0.5000x0.5000f_dst-webp_e15_p258x258_q70_tt1_u&efg=eyJ1cmxnZW4iOiJ1cmxnZW5fZnJvbV91cmwifQ&_nc_eui2=AeF9d7RnxAiaigDLCwCgzhEwyjjws-e1duzKOPCz57V27B7_7FSIlAZ1w1_lGIjoi0-6hRjcI2ClwTxCcF3FOFQ0&_nc_cid=0&_nc_ad=z-m&_nc_rml=0&_nc_ht=scontent.fmnl24-1.fna&_nc_cat=102&_nc_ohc=hIuc684Crl0AX9w2qIb&ccb=1-7&_nc_sid=5fac6f&oh=00_AfDIQXGHPkEXXh8os2sNbBeTC_C5gksj3pTabhIwMj-1Pg&oe=6512403A " class="off president"/>
                <p><span>Tristan Bajamundi</span><br />Auditor</p>
            </div>
        </div>
    </div>
    
    <div id="students">
        <h2>Aspiring Developers</h2>
        <p class="info">This section should be the list of my classmates in BSCS-2A, but I'm lazy enough to put their names. PS, the height of this section is auto, so i can add as many names as I want without losing the layout. Imma put names maybe next time.</p>
        <p class="info">Another one, I will change this section from paragraph to ul li, so that there will be a clear view to the list of names. That's all</p>
    </div>
    
    <div id="others">
        <h2>About</h2>
        <div class="misc">
            <div class="address">
                &nbsp<i class="fa-solid fa-location-dot"></i><span>&nbsp&nbspJ. Gonzales, Barangay 4, Tanauan, 4232 Batangas</span>
            </div>
            <br />
            <div class="hours">
                <i class="fa-solid fa-clock"></i> <span>&nbspDaily • Closes 5 PM</span>
            </div>
            <br />
            <div class="telephone">
                <i class="fa-solid fa-phone"></i> <span> (043) 778 1742</span>
            </div>
        </div>
        
        <div class="dev">
            <span class="smol">Developer's Info</span>
            <span class="smol">Ivan</span>
            <span class="smol">PS: not responsive. tinatamad na ako</span>
            <span class="smol">Hello kay ano hehe</span>
            
        </div>
        </div>
        

    </div>
</body>

<script>
    
    const line1 = document.querySelector('.one');
    const line2 = document.querySelector('.two');
    const line3 = document.querySelector('.three');
    const as = document.querySelectorAll('a');
    const borgar = document.querySelector('.borgar');
    
    borgar.addEventListener("click", function() {
        line1.classList.toggle("one1");
        line2.classList.toggle("two2");
        line3.classList.toggle("three3");
        as.forEach(i => {
            i.classList.toggle("asible");
        })
    })
    
</script>
</html>
