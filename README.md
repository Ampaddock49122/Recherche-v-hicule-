# Recherche-v-hicule-<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recherche de Véhicules</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            text-align: center;
            color: #333;
        }
        .form-group {
            margin-bottom: 15px;
        }
        .form-group label {
            display: block;
            color: #333;
        }
        .form-group input,
        .form-group select {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
        }
        .form-group button {
            width: 100%;
            padding: 10px;
            background-color: #007BFF;
            color: #fff;
            border: none;
            cursor: pointer;
        }
        .form-group button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Recherche de Véhicules</h2>
    <form action="/search_results" method="get">
        <div class="form-group">
            <label for="vehicleType">Type de véhicule:</label>
            <select id="vehicleType" name="vehicleType" required>
                <option value="">Sélectionner un type</option>
                <option value="car">Voiture</option>
                <option value="motorcycle">Moto</option>
                <option value="truck">Camion</option>
                <!-- Ajoutez d'autres options si nécessaire -->
            </select>
        </div>
        <div class="form-group">
            <label for="brand">Marque:</label>
            <input type="text" id="brand" name="brand" placeholder="Ex: Toyota, BMW" required>
        </div>
        <div class="form-group">
            <label for="model">Modèle:</label>
            <input type="text" id="model" name="model" placeholder="Ex: Corolla, X5" required>
        </div>
        <div class="form-group">
            <label for="year">Année:</label>
            <input type="number" id="year" name="year" min="1900" max="2024" placeholder="Ex: 2018">
        </div>
        <div class="form-group">
            <label for="price">Prix maximum (€):</label>
            <input type="number" id="price" name="price" placeholder="Ex: 20000">
        </div>
        <div class="form-group">
            <label for="mileage">Kilométrage maximum (km):</label>
            <input type="number" id="mileage" name="mileage" placeholder="Ex: 50000">
        </div>
        <div class="form-group">
            <label for="fuelType">Type de carburant:</label>
            <select id="fuelType" name="fuelType">
                <option value="">Sélectionner un type</option>
                <option value="petrol">Essence</option>
                <option value="diesel">Diesel</option>
                <option value="electric">Électrique</option>
                <option value="hybrid">Hybride</option>
            </select>
        </div>
        <div class="form-group">
            <button type="submit">Rechercher</button>
        </div>
    </form>
</div>

</body>
</html>
