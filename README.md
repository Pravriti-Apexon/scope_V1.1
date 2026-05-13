<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>APEX Clinical Dashboard</title>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>
body {
  margin:0;
  font-family: 'Segoe UI', sans-serif;
  background:#f5f7fb;
}

header {
  background: #1e3c72;
  color:white;
  padding:20px;
}

h1 { margin:0; }

.container {
  padding:20px;
}

/* Metrics */
.metrics {
  display:grid;
  grid-template-columns: repeat(auto-fit, minmax(200px,1fr));
  gap:15px;
}

.metric {
  background:white;
  border-radius:10px;
  padding:20px;
  box-shadow:0 2px 8px rgba(0,0,0,0.1);
}

.metric h3 {
  margin:0;
  color:#666;
}

.metric p {
  font-size:22px;
  font-weight:bold;
}

/* Grid */
.grid {
  display:grid;
  grid-template-columns: 2fr 1fr;
  gap:20px;
  margin-top:20px;
}

.card {
  background:white;
  padding:20px;
  border-radius:10px;
  box-shadow:0 2px 8px rgba(0,0,0,0.1);
}

/* Tabs */
.tabs {
  display:flex;
  gap:10px;
  margin-bottom:10px;
}

.tab {
  padding:10px 15px;
  background:#ddd;
  cursor:pointer;
  border-radius:5px;
}

.tab.active {
  background:#1e3c72;
  color:white;
}

.content { display:none; }
.content.active { display:block; }

/* Status colors */
.green { color:#4CAF50; }
