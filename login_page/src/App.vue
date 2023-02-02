<template >
    <main>
        <section class="login-container">
            <div class="container login">
                <p>Comece agora sua jornada no mundo <strong>dev,</strong>faça agora seu login e aproveite nosso curso <strong>gratuito!</strong></p>
                <div class="card">
                    <img src="./assets/rockt_icon.svg" alt="Imagem de Foquete">
                    <div class="box-inputs">
                        <input type="text" placeholder="username">
                        <input :type="isVisibly ? 'text':'password'" placeholder="password">
                        <a href="http://www.google.com" target="_blank" rel="noopener noreferrer">
                            Esqueceu sua senha?
                        </a>
                    </div>
                    <div class="box-button">
                        <button class="parti">Parti</button>  
                        <div class="row">Cadastre-se ></div>
                    </div>
                </div>
            </div>
            
        </section>
    </main>
</template>
<script>
export default {
    data(){
        return{
            username:"",
            isVisibly:true,
        }
    }
}
</script>
<style scoped>
    body{
        height: 100%;
    }

    #app{
        min-height: 100%;
    }

    main{
        height: 100%;
    }

    .login-container{
        height: 100%;
        background-image: url("./assets/background.svg");
        background-size:cover;
        font-family: "Rubik",sans-serif;
    }
    .login{
        padding: 180px 79px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    strong{
        color: #C8A585;
    }

    p{
        color: white;
        max-width: 682px;
        font-weight: 700;
        font-size: 3.125rem;
        line-height: 59.25px;
    }

    .card{
        padding: 54px 40px;
        font-family: "Exo",sans-serif;
        border-radius: 10px;
        background-color: #1F2635;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 36px;
    }

    .box-inputs{
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 11px;
    }

    input{
        border: none;
        background-color: #2D3545;
        border-radius: 4px;
        min-width: 273px;
        padding: 15px 16px;
        color: #C8A585;
        font-weight: 600;
        font-size: 0.75rem;
    }

    a{
        font-family: "Exo",sans-serif;
        font-weight: 600;
        font-size: 0.688rem;
        color:#C8A585;
    }

    .box-button{
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 15px;
    }

    .parti{
        border: none;
        border-radius: 4px;
        font-family: "Exo",sans-serif;
        background-color: #2D3545;
        min-width: 176px;
        padding-bottom: 10px;
        padding-top: 10px;
        font-weight: 700;
        font-size: 0.875rem;
        color: #C8A585;
        cursor: pointer;
    }

    .row{
        color:#C8A585 ;
        font-size: 12px;
        font-weight: 700;
        cursor: pointer;
    }
    
</style>