# SKRZ23.github.io
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dashboard Multi Sheet</title>

<style>
body {
    font-family: Arial;
    background: #0f172a;
    color: white;
    margin: 0;
}

.header {
    padding: 20px;
}

.tabs {
    display: flex;
    gap: 10px;
    padding: 0 20px;
}

.tab {
    padding: 10px 20px;
    background: #1e293b;
    border-radius: 8px;
    cursor: pointer;
    transition: 0.3s;
}

.tab:hover {
    background: #38bdf8;
}

.tab.active {
    background: #38bdf8;
    color: black;
}

iframe {
    width: 100%;
    height: 85vh;
    border: none;
    margin-top: 10px;
}
</style>

</head>
<body>

<div class="header">
    <h1>📊 Dashboard Data</h1>
</div>

<div class="tabs">
    <div class="tab active" onclick="gantiSheet(0)">Sheet 1</div>
    <div class="tab" onclick="gantiSheet(1)">Sheet 2</div>
    <div class="tab" onclick="gantiSheet(2)">Sheet 3</div>
</div>

<iframe id="frame" src=""></iframe>

<script>
const sheets = [
    "https://docs.google.com/spreadsheets/d/e/2PACX-1vQZsBA_TeLq6n4PrNuJCXu6wcb9pLrFgOlt5-XYeE36laNYDyAsIYZsegCpimpYqPyZgdsFnVufCPLx/pubhtml?gid=0&single=true",
    "https://docs.google.com/spreadsheets/d/e/2PACX-1vQZsBA_TeLq6n4PrNuJCXu6wcb9pLrFgOlt5-XYeE36laNYDyAsIYZsegCpimpYqPyZgdsFnVufCPLx/pubhtml?gid=123456&single=true",
    "https://docs.google.com/spreadsheets/d/e/2PACX-1vQZsBA_TeLq6n4PrNuJCXu6wcb9pLrFgOlt5-XYeE36laNYDyAsIYZsegCpimpYqPyZgdsFnVufCPLx/pubhtml?gid=789012&single=true"
];

function gantiSheet(index) {
    document.getElementById("frame").src = sheets[index];

    document.querySelectorAll(".tab").forEach(tab => tab.classList.remove("active"));
    document.querySelectorAll(".tab")[index].classList.add("active");
}

// Load pertama
gantiSheet(0);
</script>

</body>
</html>
