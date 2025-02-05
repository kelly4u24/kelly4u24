<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KenMglobal Logistics Services</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 20px; }
        header { background: #007bff; color: white; padding: 15px; font-size: 24px; }
        section { margin: 20px 0; }
        input, button { padding: 10px; margin: 10px; }
        .tracking-result { margin-top: 20px; font-size: 18px; color: green; }
    </style>
</head>
<body>
    <header>Welcome to KenMglobal Logistics Services</header>
    <section>
        <h2>About Us</h2>
        <p>We provide reliable and fast logistics solutions worldwide.</p>
        <p><strong>Motto:</strong> Logistics you can trust</p>
    </section>
    <section>
        <h2>Track Your Shipment</h2>
        <input type="text" id="trackingNumber" placeholder="Enter Tracking Number">
        <button onclick="trackShipment()">Track</button>
        <div class="tracking-result" id="trackingResult"></div>
    </section>
    <section>
        <h2>Contact Us</h2>
        <p>Email: support@kenmglobal.com</p>
        <p>Phone: 08066737202, 09136112021</p>
    </section>
    <script>
        function trackShipment() {
            var trackingNumber = document.getElementById("trackingNumber").value;
            var resultDiv = document.getElementById("trackingResult");
            if (trackingNumber) {
                resultDiv.innerHTML = "Tracking number " + trackingNumber + " is in transit.";
            } else {
                resultDiv.innerHTML = "Please enter a valid tracking number.";
            }
        }
    </script>
</body>
</html>
