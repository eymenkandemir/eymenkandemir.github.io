<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mobil Uyumlu Davetli Listesi ve Menü</title>
    <style>
        /* Genel stil ayarları */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Başlık */
        header {
            background-color: #4CAF50;
            color: white;
            padding: 1rem;
            text-align: center;
        }

        /* Konteyner */
        .container {
            display: flex;
            flex-direction: row;
            height: calc(100vh - 70px); /* Header yüksekliği çıkarılır */
        }

        /* Sol taraf: Davetli Listesi */
        .sidebar {
            width: 30%;
            background-color: #f4f4f4;
            padding: 1rem;
            overflow-y: auto;
            box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
        }

        /* Sağ taraf: Menü */
        .main-content {
            width: 70%;
            padding: 1rem;
            overflow-y: auto;
        }

        /* Davetli Listesi Başlık */
        .sidebar h2, .main-content h2 {
            margin-top: 0;
        }

        /* Mobil uyumluluk - ekran küçükse alt alta diz */
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }

            .sidebar, .main-content {
                width: 100%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Davetli Listesi ve Menü</h1>
</header>

<div class="container">
    <!-- Davetli Listesi -->
    <div class="sidebar">
        <h2>Davetli Listesi</h2>
        <ul>
            <li>Misafir 1</li>
            <li>Misafir 2</li>
            <li>Misafir 3</li>
            <li>Misafir 4</li>
            <li>Misafir 5</li>
            <!-- Daha fazla davetli ekleyebilirsiniz -->
        </ul>
    </div>

    <!-- Menü -->
    <div class="main-content">
        <h2>Menü</h2>
        <p>Yemek 1: Tavuk Şiş</p>
        <p>Yemek 2: Etli Pilav</p>
        <p>Yemek 3: Karışık Meze</p>
        <p>Yemek 4: Tatlı Çeşitleri</p>
        <!-- Menü öğelerini buraya ekleyebilirsiniz -->
    </div>
</div>

</body>
</html>
