<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Date Proposal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #fce4ec;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #d81b60;
            color: white;
            text-align: center;
            padding: 20px 0;
        }
        h1 {
            font-size: 2.5rem;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
        }
        input[type="date"], input[type="time"] {
            width: 100%;
            padding: 10px;
            font-size: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        button {
            background-color: #d81b60;
            color: white;
            border: none;
            padding: 15px 20px;
            font-size: 1.2rem;
            cursor: pointer;
            border-radius: 5px;
            width: 100%;
        }
        button:hover {
            background-color: #c2185b;
        }
        footer {
            background-color: #d81b60;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

<header>
    <h1>Camille's proposal valentine date</h1>
    <p>Would you like to go on a special date with me?</p>
</header>

<div class="container">
    <form id="proposalForm">
        <div class="form-group">
            <label for="date">Select the Date</label>
            <input type="date" id="date" name="date" required>
        </div>

        <div class="form-group">
            <label for="time">Select the Time</label>
            <input type="time" id="time" name="time" required>
        </div>

        <div class="form-group">
            <label for="message">Your Special Message</label>
            <textarea id="message" name="message" rows="4" required placeholder="Write your message here..."></textarea>
        </div>

        <button type="submit">Propose the Date</button>
    </form>
</div>

<footer>
    <p>&hearts; Please make screenshot after submitting and send to your partner</p>
</footer>

<script>
    document.getElementById("proposalForm").addEventListener("submit", function(event) {
        event.preventDefault();
        const date = document.getElementById("date").value;
        const time = document.getElementById("time").value;
        const message = document.getElementById("message").value;

        alert(`Proposal sent!\n\nDate: ${date}\nTime: ${time}\nMessage: ${message}`);
    });
</script>

</body>
</html>
