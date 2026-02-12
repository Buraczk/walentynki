# walentynki
<!DOCTYPE html>
<html lang="pl">
<head>
<meta charset="UTF-8">
<title>💖 Zostaniesz moją walentynką? 💖</title>
<style>
    body {
        margin: 0;
        padding: 0;
        overflow: hidden;
        font-family: 'Arial', sans-serif;
        background: linear-gradient(135deg, #ed226c, #ef728f);
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .container {
        position: relative;
        z-index: 2;
        text-align: center;
        background: rgba(255,255,255,0.85);
        padding: 30px 40px;
        border-radius: 20px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }

    h1 {
        color: #e6005c;
        margin-bottom: 20px;
    }

    .photo {
        width: 200px;
        height: 200px;
        border-radius: 20px;
        background: #ddd;
        margin: 0 auto 20px;
        background-image: url("IMG_1527.JPG"); /* <- ZMIEŃ NA SWOJE ZDJĘCIE */
        background-size: cover;
        background-position: center;
    }

    .buttons {
        margin-top: 20px;
    }

    button {
        font-size: 20px;
        padding: 10px 25px;
        margin: 10px;
        border: none;
        border-radius: 30px;
        cursor: pointer;
        transition: 0.2s;
    }

    #yesBtn {
        background: #f42a5d;
        color: white;
    }

    #yesBtn:hover {
        transform: scale(1.1);
    }

    #noBtn {
        background: #555;
        color: white;
        position: absolute;
    }

    /* Latające serca */
    .heart {
        position: absolute;
        color: #d9073b;
        font-size: 80px;
        animation: floatUp 6s linear infinite;
        opacity: 1;
    }

    @keyframes floatUp {
        0% {
            transform: translateY(100vh) scale(0.5);
            opacity: 0;
        }
        10% {
            opacity: 1;
        }
        100% {
            transform: translateY(-10vh) scale(1.2);
            opacity: 0;
        }
    }

    .musicHint {
        position: fixed;
        bottom: 10px;
        left: 50%;
        transform: translateX(-50%);
        background: rgba(0,0,0,0.6);
        color: white;
        padding: 8px 15px;
        border-radius: 20px;
        font-size: 14px;
        z-index: 5;
    }
</style>
</head>
<body>
