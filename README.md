<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Call and SMS Example</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            padding: 20px;
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            color: #ffffff;
            background-color: #007bff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h1>Call and SMS Example</h1>
    <button onclick="callAndSendMessage('+7013608114')">Call and Send SMS</button>

    <script>
        function callAndSendMessage(number) {
            // Call the number
            window.location.href = `tel:${number}`;

            // For sending SMS, you would typically use a server-side service or API.
            // This is a placeholder for where you might handle SMS sending:
            // Example: 
            // sendSMS(number, "Hello! This is a test message.");

            console.log(`SMS would be sent to ${number} with a test message.`);
        }

        // Mock function for SMS sending
        function sendSMS(number, message) {
            // Here you would typically make an API call to an SMS service
            // Example using fetch (pseudo-code):
            // fetch('https://api.sms-service.com/send', {
            //     method: 'POST',
            //     headers: {
            //         'Content-Type': 'application/json',
            //     },
            //     body: JSON.stringify({ number, message }),
            // })
            // .then(response => response.json())
            // .then(data => console.log('SMS sent:', data))
            // .catch(error => console.error('Error sending SMS:', error));
        }
    </script>
</body>
</html>
