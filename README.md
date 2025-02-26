<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #000000;
            color: #fff;
            font-family: Arial, Helvetica, sans-serif;
        }

        section {
            width: 100%;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            max-width: 800px;
            text-align: center;
        }

        h1 {
            font-size: 40px;
            margin-bottom: 1.5rem;
            padding: 20px;
        }
        h5 {
            font-family: 'Roboto', Times, serif;
            font-size: 2.5rem;
        }

        p {
            font-size: 1.9rem;
            margin-bottom: 10px;
            line-height: 1.5;
            padding: 20px;
            font-family: 'Roboto', Times, serif;
            margin-top: 20px;
        }

        .li-p {
            font-size: 1.7rem;
        }

        .inicio-li {
            padding-top: 35px;
            text-decoration: none;
        }

        @media (max-width: 600px) {
            h5 {
                font-size: 1.5rem;
            }

            .li-p {
                font-size: 1rem;
            }
        }
        @media (max-width: 1024px) {
            h5 {
                font-size: 2.9rem;
                
            }

            .li-p {
                font-size: 2.rem;
            }
        }

        .imagens {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
            gap: 10px;
            margin-top: 10px;
            
        }

        .imagens img {
            width: 500px;
            height: auto;
            border-radius: 20px;

        }

        @media (max-width: 600px) {
            h1 {
                font-size: 30px;
            }

            p {
                font-size: 18px;
            }
        }

        .item img {
            width: 50rem;
            height: auto;
            border-radius: 5px;
            padding-top: 10px;
        }


        .carousel-inner {
            display: flex;
            justify-content: center;
            align-items: center;
            padding-top: 10px;
        }

        .carousel-indicators {
            transform: translateY(20px);
        }

        .footer {
            margin-top: 20px;
            text-align: center;
        }
    </style>
</head>

<body>
    <section>
        <div class="container">
            <h1>Projeto Easy-Car</h1>
            <p>
                O EasyCar é uma forma inteligente de transporte que visa unir motoristas e passageiros,
                facilitando a comunicação entre oferta de viagens e usuários.
            </p>
            <p>
                <strong>Descrição:</strong> <br>
                EasyCar Mobile é um aplicativo desenvolvido com React Native e Expo, projetado para facilitar a
                localização de carros e interação com mapas, permitindo que motoristas e passageiros se comuniquem
                facilmente.
                Interface simples intíitiva.
            </p>
            <p>
                <strong>Tecnologias utilizadas:</strong> <br>
                React Native | Expo | React Navigation | React Native Maps
            </p>
            <p>
                <strong>Funcionalidades Principais:</strong> <br>
                <strong>Localização em Tempo Real:</strong> Uso de expo-location e react-native-maps.<br>
                <strong>Navegação:</strong> Implementado com @react-navigation/native e
                @react-navigation/native-stack.<br>
                <strong>Interface Amigável:</strong> Desenvolvido para ser responsivo e intuitivo.<br>
                <strong>Segurança:</strong> Integração com react-native-safe-area-context.
            </p>

            <div>
                <p><strong>Imagens do projeto</strong></p>
                <div class="imagens">
                    <div>
                        <div id="myCarousel" class="carousel slide" data-ride="carousel">
                            <!-- Indicators -->
                            <ol class="carousel-indicators">
                                <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
                                <li data-target="#myCarousel" data-slide-to="1"></li>
                                <li data-target="#myCarousel" data-slide-to="2"></li>
                                <li data-target="#myCarousel" data-slide-to="3"></li>
                                <li data-target="#myCarousel" data-slide-to="4"></li>

                            </ol>

                            <!-- Wrapper for slides -->
                            <div class="carousel-inner">
                                <div class="item active">
                                    <img src="./src/assents/tela-inicial.png" alt="Los Angeles">
                                </div>

                                <div class="item">
                                    <img src="./src/assents/tela-home.png" alt="Chicago">
                                </div>

                                <div class="item">
                                    <img src="./src/assents/passenger-corrida-aceita.png" alt="New York">
                                </div>
                                <div class="item">
                                    <img src="./src/assents/tela-ride.png" alt="New York">
                                </div>
                            </div>

                            <!-- Left and right controls -->
                            <a class="left carousel-control" href="#myCarousel" data-slide="prev">
                                <span class="glyphicon glyphicon-chevron-left"></span>
                                <span class="sr-only">Previous</span>
                            </a>
                            <a class="right carousel-control" href="#myCarousel" data-slide="next">
                                <span class="glyphicon glyphicon-chevron-right"></span>
                                <span class="sr-only">Next</span>
                            </a>
                        </div>
                    </div>
                    <div class="inicio-li">
                        <h5>Iniciando o projeto</h5>
                        <ul>
                            <li>
                                <p class="li-p">
                                    Pasta mobile :<span><br>npm install<br>npx expo start</span> 
                                </p>
                            </li>
                            <li>
                                <p class="li-p">
                                    Pasta servidor-api :<span><br>npm install<br>node --watch src/index.js</span> 
                                </p>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <div class="footer">
                <p class="p"><strong>Desenvolvido por:</strong> <br> Leandro Pereira Martins</p>
                
            </div>
        </div>
    </section>
</body>

</html>
