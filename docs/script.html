<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Map of Bristol with EV Charging Points</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: row;
            background-color: #f8f8f8;
        }
        #map-container {
            width: 70%;
            height: 100vh;
            position: relative;
            box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.1);
        }
        iframe {
            width: 100%;
            height: 100%;
            border: none;
            border-radius: 8px;
        }
        #data-container {
            width: 30%;
            height: 100vh;
            overflow-y: auto;
            padding: 20px;
            background-color: #ffffff;
            box-shadow: -3px 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            margin-left: 10px;
        }
        h2 {
            font-size: 26px;
            margin-bottom: 15px;
            color: #333;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 20px;
            border-radius: 8px;
            overflow: hidden;
        }
        th, td {
            padding: 12px;
            border-bottom: 1px solid #ddd;
            text-align: left;
            font-size: 14px;
        }
        th {
            background-color: #007bff;
            color: white;
        }
        tr:hover {
            background-color: #f1f1f1;
        }
        .loading {
            font-size: 18px;
            text-align: center;
            color: #888;
        }
        #searchInput {
            padding: 10px;
            width: 100%;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 14px;
            background-color: #f9f9f9;
        }
        #searchInput:focus {
            outline: none;
            border-color: #007bff;
        }
    </style>
</head>
<body>
    <div id="map-container">
        <iframe id="bristolMap" src="" frameborder="0" allowfullscreen></iframe>
    </div>
    <div id="data-container">
        <input type="text" id="searchInput" placeholder="Search Charging Points...">
        <h2>Charging Points</h2>
        <table id="charging-points-table">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Description</th>
                    <th>Address</th>
                </tr>
            </thead>
            <tbody id="charging-points-body">
                <tr>
                    <td colspan="3" class="loading">Loading charging points...</td>
                </tr>
            </tbody>
        </table>
    </div>

    <script>
        async function loadMapWithChargingPoints() {
            const apiUrl = 'https://maps2.bristol.gov.uk/server2/rest/services/ext/ll_transport/MapServer/21/query?where=LocationType%3D%27Electric%20Vehicle%20Charging%20Point%27&outFields=*&outSR=4326&f=json';

            try {
                const response = await fetch(apiUrl);
                const data = await response.json();

                if (data.error) {
                    throw new Error(`API Error: ${data.error.message}`);
                }

                const chargingPoints = data.features;

                const iframe = document.getElementById('bristolMap');
                iframe.src = 'https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2482.328828372484!2d-2.597298684229292!3d51.45451327962831!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x48718f4a5a3290d5%3A0x1ec4c60792f47ba9!2sBristol!5e0!3m2!1sen!2suk!4v1620324174311!5m2!1sen!2suk';

                const chargingPointsBody = document.getElementById('charging-points-body');
                chargingPointsBody.innerHTML = ''; // Clear the table body

                chargingPoints.forEach(point => {
                    const name = point.attributes.DeviceName;
                    const description = point.attributes.LocationShDesc;
                    const address = `${point.attributes.BuildingNumber} ${point.attributes.Thoroughfare}, ${point.attributes.PostTown}, ${point.attributes.PostCode}`;

                    const row = document.createElement('tr');
                    row.innerHTML = `
                        <td>${name}</td>
                        <td>${description}</td>
                        <td>${address}</td>
                    `;
                    chargingPointsBody.appendChild(row);
                });
            } catch (error) {
                console.error('Error fetching data:', error);
            }
        }

        document.getElementById('searchInput').addEventListener('input', function() {
            const filter = this.value.toLowerCase();
            const rows = document.querySelectorAll('#charging-points-body tr');
            rows.forEach(row => {
                const name = row.cells[0].textContent.toLowerCase();
                const description = row.cells[1].textContent.toLowerCase();
                const address = row.cells[2].textContent.toLowerCase();
                if (name.includes(filter) || description.includes(filter) || address.includes(filter)) {
                    row.style.display = '';
                } else {
                    row.style.display = 'none';
                }
            });
        });

        window.onload = loadMapWithChargingPoints;
    </script>
</body>
</html>
