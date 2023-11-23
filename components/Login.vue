
<template class="teste">

    <div class="primeira">

        <form class="form">

            <img src="../img/teste.png" width="250" height="30" alt="logotipo">

            <h1> Cadastrar  </h1>

            <label>
                <span> E-mail </span>
                <input type="email" name="email">
            </label>

            <label>
                <span> Senha </span>
                <input type="passoword" name="password">
            </label>

            <button class="submit" type="button"> Cadastrar </button>

        </form>

    </div>

    <div class="segunda">

<form class="form">

    <h1> Logar </h1>

    <label>
        <span> Email </span>
        <input type="email" name="email">
    </label>

    <label>
        <span> Senha </span>
        <input type="passoword" name="password">
    </label>

    <button class="submit" type="button"> Login </button>

</form>

</div>

</template>

<script>

</script>

<style>

body{
    background-color: #2F3A4B;
}
.primeira{
        display: inline-block;
        background: #fff;
        box-shadow: 0 19px 38px black, 0 15px 12px rgba(0, 0, 0, 0.22);
        border-radius: 25px;
        width: 40%;
        position: absolute;
        top: 50%;
        left: 40%;
        transform: translate(-50%, -50%);
    }

.segunda{
        display: inline-block;
        background: #fff;
        box-shadow: 0 19px 38px black, 0 15px 12px rgba(0, 0, 0, 0.22);
        border-radius: 25px;
        widows: 40%;
        margin-left: 350px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    h1{
        color: black;
        padding-top: 10px;
        font-size: 30px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        text-align: center;
    }

    .form{
        padding: 50px 30px;
        -webkit-transition: -webkit-tranform 1.2s ease-in-out;
        transition:  -webkit-tranform 1.2s ease-in-out;
        transition:  trasnform 1.2s ease-in-out;
        transition:  trasnform 1.2s ease-in-out, -webkit-tranform 1.2s ease-in-out;
    }

    label {
        display: block;
        width: 260px;
        margin: 25px auto 0;
        text-align: center;
    }

    label span {
        font-size: 14px;
        font-weight: 600;
        color: rgb(0, 0, 0);
        text-transform: uppercase;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    input{
        display: block;
        width: 100%;
        margin-top: 5px;
        font-size: 16px;
        padding-bottom: 1px solid rgba(109, 93, 93, 0.4);
        text-align: center;
        font-family: 'Nunito', sans-serif;

    }

    button{
        display: block;
        margin: 20px auto;
        width: 260px;
        height: 36px;
        border-radius: 30px;
        background-color: #2F3A4B;
        font-size: 15px;
        cursor: pointer;
        color: #fff;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    button:hover{
        background-color: #865CD0;
    }

</style>