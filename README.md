<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Location Information</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
        }
        .container {
            max-width: 800px;
            margin: auto;
        }
        h1 {
            text-align: center;
            color: #333;
        }
        .info {
            margin: 20px 0;
            padding: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #f9f9f9;
        }
        .info h2 {
            margin-top: 0;
            color: #555;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Location Information for ZIP Code 12503</h1>
        <div class="info">
            <h2>Average Annual Salary</h2>
            <p id="salary">Loading...</p>
        </div>
        <div class="info">
            <h2>Average Home Price</h2>
            <p id="homePrice">Loading...</p>
        </div>
        <div class="info">
            <h2>Rent vs. Own Percentage</h2>
            <p id="rentOwn">Loading...</p>
        </div>
        <div class="info">
            <h2>Average Annual Snowfall</h2>
            <p id="snowfall">Loading...</p>
        </div>
    </div>
    <script>
        async function fetchData(zipCode) {
            // Placeholder for fetching real data
            const mockData = {
                salary: "$60,000",
                homePrice: "$300,000",
                rentOwn: "40% Rent / 60% Own",
                snowfall: "50 inches"
            };

            document.getElementById('salary').textContent = mockData.salary;
            document.getElementById('homePrice').textContent = mockData.homePrice;
            document.getElementById('rentOwn').textContent = mockData.rentOwn;
            document.getElementById('snowfall').textContent = mockData.snowfall;
        }

        fetchData("12503");
    </script>
</body>
</html>
