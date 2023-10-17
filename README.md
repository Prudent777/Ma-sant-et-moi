# Ma-sant-et-moi
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Montserrat", sans-serif;
    scroll-behavior: smooth;
}

.home-container {
    min-height: 100vh;
    background: url(images/bg.jpg);
    background-size: cover;
}

.header {
    position: absolute;
    width: 100%;
    height: 150px;
    display: flex;
    align-items: center;
    padding: 0 50px;
}

.logo {
    width: 180px;
}

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li {
    margin: 40px;
    overflow: hidden;
}

.nav-links a {
    font-size: 15px;
    font-weight: 500;
    color: white;
    text-decoration: none;
    position: relative;
    display: block;
    transition: transform 0.4s;
}

.nav-links a::before {
    content: attr(data-text);
    position: absolute;
    top: 100%;
}

.nav-links a:hover {
    transform: translateY(-100%);
}

.burger {
    display: none;
}

.landing {
    line-height: 80px;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 100px;
}

.big-title {
    width: 40%;
    color: white;
    font-size: 80px;
    font-family: "Abril Fatface", cursive;
    font-weight: 100;
}

.delivery-link {
    line-height: 20px;
    text-decoration: none;
    display: flex;
    align-items: center;
    position: absolute;
    bottom: 30px;
    width: 70px;
    justify-content: space-between;
    overflow: hidden;
}

.scroll-text {
    color: white;
    position: relative;
    transition: transform 0.4s;
}

.scroll-text::before {
    content: attr(data-text);
    position: absolute;
    top: 100%;
}

.scroll-text:hover {
    transform: translateY(-100%);
}

.scroll-icon {
    font-size: 25px;
    color: white;
}

.delivery-container {
    min-height: 300px;
    background: white;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}

.delivery-container div {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.delivery-icon {
    font-size: 50px;
    color: #ADD981;
}

.delivery-container .box-content {
    font-weight: 500;
    font-size: 20px;
    margin-top: 30px;
    width: 220px;
    text-align: center;
}

.best-sales-container {
    min-height: 80vh;
    background: white;
    padding: 0 100px;
}

.section-title {
    position: relative;
    font-family: "Abril Fatface", cursive;
    font-size: 50px;
    font-weight: 100;
}

.section-title::before {
    content: "";
    position: absolute;
    width: 50px;
    height: 7px;
    background: #ADD981;
    bottom: 0;
    box-shadow: 0 2px 2px #0000001F;
}

.best-plants {
    display: flex;
    margin-top: 50px;
    flex-wrap: wrap;
    justify-content: center;
}

.plant1 {
    background: url(images/nos_meilleures_ventes/1.jpg);
}

.plant2 {
    background: url(images/nos_meilleures_ventes/2.jpg);
}

.plant3 {
    background: url(images/nos_meilleures_ventes/3.jpg);
}

.plant4 {
    background: url(images/nos_meilleures_ventes/4.jpg);
}

.plant-box::before {
    content: "En savoir plus";
    position: absolute;
    width: 100%;
    height: 100%;
    background: #FFFFFFDF;
    display: flex;
    justify-content: center;
    align-items: center;
    left: -100%;
    transition: left 0.4s;
    font-size: 25px;
    font-weight: 500;
}

.plant-box:hover::before {
    left: 0;
}

.plant-bio {
    position: absolute;
    bottom: 0;
    display: flex;
    background: #FFFFFFDF;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    padding: 15px 20px;
    flex-wrap: wrap;
}

.plant-name {
    font-weight: 500;
    font-size: 30px;
}

.plant-price {
    font-weight: 300;
    font-size: 15px;
}

.plants-container {
    padding: 0 100px;
    min-height: 150vh;
    margin-top: 50px;
}

.grid-plants {
    margin-top: 50px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(4, 400px);
}

.plant-grid1 {
    background: url(images/nos_plantes/1.jpg);
    grid-column: 1 / 3;
    grid-row: 1 / 3;
}

.plant-grid2 {
    background: url(images/nos_plantes/2.jpg);
    grid-column: 3 / 5;
}

.plant-grid3 {
    background: url(images/nos_plantes/3.jpg);
    grid-column: 3 / 5;
}

.plant-grid4 {
    background: url(images/nos_plantes/4.jpg);
    grid-column: 1;
    grid-row: 3 / 5;
}

.plant-grid5 {
    background: url(images/nos_plantes/5.jpg);
    grid-column: 2 / 4;
    grid-row: 3 / 5;
}

.plant-grid6 {
    background: url(images/nos_plantes/6.jpg);
    grid-column: 4;
    grid-row: 3 / 5;
}

.plant-box {
    position: relative;
    background-size: cover;
    background-position: center;
    cursor: pointer;
    text-decoration: none;
    color: black;
    overflow: hidden;
    transition: background 0.4s;
}

.no-grid {
    height: 500px;
    flex: 1;
    min-width: 350px;
}

.footer {
    min-height: 100px;
    display: flex;
    align-items: center;
    margin-top: 50px;
    justify-content: space-between;
    padding: 0 100px;
    flex-wrap: wrap;
}

.copyrights {
    padding-right: 20px;
}

.conditions {
    color: black;
    text-decoration: none;
    font-weight: 600;
}

@media (max-width: 1150px) {

    .header {
        justify-content: space-between;
    }

    .burger-container {
        width: 35px;
        height: 30px;
        position: relative;
    }

    .burger {
        display: block;
        height: 3px;
        width: 30px;
        background: white;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        transition: background 0.4s;
    }

    .burger-container.active .burger {
        background: transparent;
    }

    .burger::before {
        content: "";
        position: absolute;
        width: 100%;
        height: 100%;
        background: white;
        bottom: 8px;
        transition: transform 0.4s,
            bottom 0.4s,
            background 0.4s;
    }

    .burger-container.active .burger::before {
        bottom: 0;
        transform: rotate(-45deg);
        background: black;
    }

    .burger::after {
        content: "";
        position: absolute;
        width: 100%;
        height: 100%;
        background: white;
        top: 8px;
        transition: transform 0.4s,
            top 0.4s background 0.4s;
    }

    .burger-container.active .burger::after {
        top: 0;
        transform: rotate(45deg);
        background: black;
    }

    .nav-links {
        position: absolute;
        width: 100%;
        height: 50vh;
        background: white;
        left: 0;
        top: -50vh;
        transition: top 0.4s ease-in-out;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: flex-start;
        padding: 0 50px;
    }

    .nav-links.active {
        top: 0;
    }

    .nav-links li {
        margin: 0;
    }

    .nav-links a {
        color: black;
        font-size: 30px;
    }

    .delivery-container {
        flex-direction: column;
        justify-content: center;
        padding: 50px;
    }

    .delivery-container div {
        margin: 30px;
    }

    .grid-plants {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .grid {
        flex: 1;
        min-width: 350px;
        height: 500px;
    }
}

@media (max-width: 550px) {

    .logo {
        width: 100px;
    }

    .landing,
    .header,
    .best-sales-container,
    .plants-container,
    .footer {
        padding: 0 7%;
    }

    .header {
        height: 100px;
    }

    .big-title {
        font-size: 50px;
        line-height: 50px;
    }

    .nav-links a {
        font-size: 20px;
    }

    .section-title {
        font-size: 30px;
        text-align: center;
    }

    .plant-box {
        min-width: 300px;
    }

    .plant-name,
    .plant-box::before {
        font-size: 20px;
    }

    .plant-price {
        font-size: 10px;
    }

}

@media (max-width: 400px) {

    .footer {
        justify-content: center;
    }
}
