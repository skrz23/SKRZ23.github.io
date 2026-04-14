# SKRZ23.github.io
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dashboard Data</title>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Segoe UI', sans-serif;
    }

    body {
        display: flex;
        background-color: #0f172a;
        color: white;
    }

    /* Sidebar */
    .sidebar {
        width: 220px;
        height: 100vh;
        background: #020617;
        padding: 20px;
    }

    .sidebar h2 {
        margin-bottom: 30px;
        color: #38bdf8;
    }

    .sidebar a {
        display: block;
        margin: 15px 0;
        color: #94a3b8;
        text-decoration: none;
        transition: 0.3s;
    }

    .sidebar a:hover {
        color: #38bdf8;
    }

    /* Main */
    .main {
        flex: 1;
        padding: 20px;
    }

    .header {
        margin-bottom: 20px;
    }

    .header h1 {
        font-size: 24px;
    }

    /* Card */
    .card {
        background: #020617;
        padding: 20px;
        border-radius: 12px;
        box-shadow: 0 0 15px rgba(0,0,0,0.3);
    }

    /* Iframe */
    iframe {
        width: 100%;
        height: 600px;
        border: none;
        border-radius: 10px;
    }

    /* Responsive */
    @media (max-width: 768px) {
        .sidebar {
            display: none;
        }
    }
</style>
</head>

<body>

<div class="sidebar">
    <h2>📊 Dashboard</h2>
    <a href="#">Home</a>
    <a href="#">Data</a>
    <a href="#">Laporan</a>
</div>

<div class="main">
    <div class="header">
        <h1>Dashboard Google Sheets</h1>
        <p>Data realtime dari spreadsheet</p>
    </div>

    <div class="card">
        <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQZsBA_TeLq6n4PrNuJCXu6wcb9pLrFgOlt5-XYeE36laNYDyAsIYZsegCpimpYqPyZgdsFnVufCPLx/pubhtml?widget=true&headers=false"></iframe>
    </div>
</div>

</body>
</html>
