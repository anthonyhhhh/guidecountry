*,
::before,
::after{
    box-sizing: border-box;
    border-width: 0;
    border-style: solid;
}
*{
    margin: 0;
}
::before, ::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}


.icon {
    position: absolute;
    color: white;
    left: 66%;
    cursor: pointer;
    top: 27%;
    width: 3rem;
    opacity: 0.6;
    transition: ease-in-out 0.4s;
}

.icon:hover{
    background-color: antiquewhite;
    color: gray;
    border-radius: 0.4rem;
} 

.brackground-image {
    position: relative;
    display: inline-block;
    text-align: center;
    justify-content: center;
}

#country-text {
    left: 35%;
    position: absolute;
    top: 8.5rem;
    color: aliceblue;
    font-size: 3rem;
    opacity: 0.5;
    font-family: 'IBM Plex Sans', sans-serif;
}

#input {
    height: 2rem;
    color: gray;
    position: absolute;
    font-size: 1.7em;
    opacity: 0.5;
    display: flex;
    outline: none;
    background-color: antiquewhite;
    border-radius: 0.5rem;
    padding: 0.5rem;
    transition: all 0.15s ease-in-out;
}

#main-container{
    position: absolute;
    width: 90%;
    height: 100vh;
    font-family: 'Inter', sans-serif;
    font-family: 'Open Sans', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
}
#draw{
    width: 100%;
    height: 10rem;
    position: absolute;
}


#input-container{
    display: flex;
    border-radius: 0.5rem;
    gap: 0.2rem;
    padding: 0.3rem;
    width: 75%;
}
#input{
    outline: none;
    width: 100%;
    color: black;
    background-color: #F2F2F2;
    border-radius: 0.3rem;
}
.search-icon{
    width: 1rem;
}
.info-container{
    width: 80%;
    height: 15rem;
    border: 1px solid greenyellow;
    display: none;
}
.info{
    width: 100%;
    height: 100%;
}
h2{
    text-align: center;
}
#country-container{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;
    padding: 0rem;
    gap: 1rem;
}
.country-card{
    display: flex;
    height: auto;
    flex-direction: column;
    width: 5rem;
    gap: 1.5rem;
}
.country-name{
    text-align: center;
    align-self: center;
    font-size: 0.6rem;
}
.flag{
    height: 50%;
    width: 100%;
    align-self: center;
    background-color: #F2F2F2;
}
.unique-card{
    display: flex;
    align-items: center;
    background-color: white;
    border-radius: 0.5rem;
    gap: 0.3rem;
    flex-direction: column;
    width: auto;
    height: 14rem;
    opacity: 0.6;
    align-self: center;
    padding: 0.8rem 0.8rem 0rem 0.8rem;
    font-size: 0.8rem;
}
.unique-flag{
    height: 30%;
    width: auto;
}

@media (max-width: 500px) {
    
    #input {
        width: 70%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #main-container{
        width: 80%;
    }
    #country-text {
        left: 2rem;
        right: 2rem;
    }
}
@media (min-width: 768px){
    #main-container{
        width: 75%;
    }
    .country-card{
        width: 6rem;
    }
    .country-name{
        font-size: 1rem;
    }
    .unique-card{
        font-size: 0.9rem;
    }
}
@media (min-width: 1024px) {
    #main-container{
        width: 60%;
    }
    .country-card{
        width: 9rem;
    }
    #draw{
        height: 15rem;
    }
    h1{
        font-size: 2rem;
    }
    #input{
        height: 1.5rem;
    }
    .search-icon{
        width: 1.8rem;
    }
}
@media (min-width: 1440px) {
    #main-container{
        width: 50%;
    }
}