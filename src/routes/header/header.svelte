<header>
    Sarah's Blog

    <img src="birch.jpg" alt="Birch"/>
</header>

<style>
    /* Default styling is mobile */
    
    header {
        background-color: #395E43;
        padding: 8px;
        color: white;
        height: 30px;
        
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    img {
        height: 100%;
    }

    /* Tablet */
    @media only screen and (min-width: 500px) {
        header {
            height: 50px;
            font-size: 25px;
        }
    }

    /* Desktop */
    @media only screen and (min-width: 800px) {
        header {
            height: 70px;
            font-size: 40px;
        }
    }
</style>