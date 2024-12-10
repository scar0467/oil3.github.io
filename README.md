<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Магазин автомобильных масел</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }
        .container {
            padding: 16px;
        }
        .card {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin: 16px 0;
            padding: 16px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .card img {
            width: 100%;
            max-width: 150px;
            border-radius: 8px;
        }
        .card h3 {
            margin: 12px 0 8px;
        }
        .card p {
            margin: 0 0 12px;
        }
        .details-btn {
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 8px 16px;
            cursor: pointer;
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
        }
        .modal-content {
            background-color: white;
            border-radius: 8px;
            padding: 16px;
            width: 90%;
            max-width: 400px;
            position: relative;
        }
        .close-btn {
            position: absolute;
            top: 8px;
            right: 8px;
            background: none;
            border: none;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="card">
            <img src="https://w7.pngwing.com/pngs/890/55/png-transparent-motor-oil-exxonmobil-lubricant-lubricant-motorcycle-oil-engine-thumbnail.png" alt="Масло 1" class="product-image" alt="Масло 1">
            <h3>Масло 1</h3>
            <p>Синтетическое, 5W-30</p>
            <button class="details-btn" onclick="openModal('modal1')">Подробности</button>
        </div>
        <div class="card">
            <img src="https://w7.pngwing.com/pngs/297/514/png-transparent-motorcycle-exxonmobil-motor-oil-lubricant-motorcycle-motorcycle-oil-engine-thumbnail.png" alt="Масло 2" class="product-image" alt="Масло 2">
            <h3>Масло 2</h3>
            <p>Полусинтетическое, 10W-40</p>
            <button class="details-btn" onclick="openModal('modal2')">Подробности</button>
        </div>
        <!-- Добавьте дополнительные карточки по аналогии -->
    </div>

    <div class="modal" id="modal1">
        <div class="modal-content">
            <button class="close-btn" onclick="closeModal('modal1')">×</button>
            <h3>Масло 1</h3>
            <p>Полное описание и характеристики масла 1.</p>
        </div>
    </div>

    <div class="modal" id="modal2">
        <div class="modal-content">
            <button class="close-btn" onclick="closeModal('modal2')">×</button>
            <h3>Масло 2</h3>
            <p>Полное описание и характеристики масла 2.</p>
        </div>
    </div>

    <script>
        function openModal(modalId) {
            document.getElementById(modalId).style.display = 'flex';
        }
        function closeModal(modalId) {
            document.getElementById(modalId).style.display = 'none';
        }
    </script>

</body>
</html>
