<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Beranda Garden</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f7fdf6; color: #333; }
    header { background: #4caf50; color: white; text-align: center; padding: 1rem; }
    h1, h2, h3 { margin: 0.5rem 0; }
    .section { padding: 2rem; }
    .plants-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 1.5rem; }
    .plant-card { background: white; border-radius: 10px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); padding: 1rem; cursor: pointer; transition: transform 0.2s; }
    .plant-card:hover { transform: translateY(-5px); }
    .plant-card img { width: 100%; height: 150px; object-fit: cover; border-radius: 8px; }
    .plant-details { display: none; background: white; padding: 2rem; position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); max-width: 600px; width: 90%; border-radius: 10px; box-shadow: 0 4px 12px rgba(0,0,0,0.2); z-index: 10; overflow-y: auto; max-height: 80vh; }
    .overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.5); z-index: 5; }
    .close-btn { float: right; cursor: pointer; font-weight: bold; }
    p { margin: 0.5rem 0; }
  </style>
</head>
<body>

<header>
  <h1>🌿 My Beranda Garden 🌸</h1>
</header>

<div class="section">
  <h2>Belongs to Me</h2>
  <div class="plants-grid">
    <div class="plant-card" onclick="showDetails('spider')">
      <img src="spider_plant.jpg" alt="Spider Plant">
      <h3>Spider Plant 🕷️</h3>
      <p>Chlorophytum comosum</p>
    </div>
    <div class="plant-card" onclick="showDetails('crown')">
      <img src="crown_of_thorns.jpg" alt="Crown of Thorns">
      <h3>Crown of Thorns 🌵</h3>
      <p>Euphorbia milii</p>
    </div>
    <div class="plant-card" onclick="showDetails('jasmine')">
      <img src="arabian_jasmine.jpg" alt="Arabian Jasmine">
      <h3>Arabian Jasmine 🌸</h3>
      <p>Jasminum sambac</p>
    </div>
    <div class="plant-card" onclick="showDetails('moss')">
      <img src="moss_rose.jpg" alt="Moss Rose">
      <h3>Moss Rose 🌺</h3>
      <p>Portulaca grandiflora</p>
    </div>
    <div
