<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>APEX Dashboard</title>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>
body { margin:0; font-family: Arial; background:#f2f4f8; }

header {
  background: linear-gradient(90deg,#1e3c72,#2a5298);
  color:white;
  padding:20px;
  text-align:center;
}

.container { padding:20px; }

.cards { display:flex; gap:15px; flex-wrap:wrap; }

.card {
  flex:1; min-width:200px;
  padding:20px;
  border-radius:10px;
  color:white;
}

.green{background:#4CAF50;}
.orange{background:#ff9800;}
.blue{background:#2196F3;}
.red{background:#f44336;}

.tabs { display:flex; gap:10px; margin-top:20px; }

.tab {
  padding:10px 15px;
  background:#ddd;
  cursor:pointer;
  border-radius:5px;
}

.tab.active { background:#2a5298; color:white; }

.content { display:none; background:white; padding:20px; margin-top:10px; border-radius:10px; }
.content.active { display:block; }

.accordion {
  margin-top:10px;
  background:#eee;
  padding:10px;
  cursor:pointer;
}

.panel {
  display:none;
  padding:10px;
  background:#fafafa;
}
</style>
</head>

<body>

<header>
<h1>APEX Clinical Platform</h1>
<p>Interactive Dashboard</p>
</header>

<div class="container">

