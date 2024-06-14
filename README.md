<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pharmacy Management System</title>
    <link rel="stylesheet" href="sty123.css">
</head>
<body>
    <header>
        <img src="pharma.png" alt="Pharmacy Logo" class="header-logo">
        <h1>Pharmacy Management System</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#" onclick="showPage('medicine-database')">Medicine Database</a></li>
            <li><a href="#" onclick="showPage('medicine-management')">Medicine Management</a></li>
            <li><a href="#" onclick="showPage('stock-management')">Stock Management</a></li>
        </ul>
    </nav>
    <main>
        <section id="medicine-database" class="page">
            <h2>Medicine Database</h2>
            <div class="medicine-info">
                <label for="search">Search Medicine:</label>
                <input type="text" id="search" placeholder="Enter medicine name">
                <button onclick="searchMedicine()">Search</button>
            </div>
            <div id="medicine-list" class="content-box">
                <!-- Dynamic content will be loaded here -->
            </div>
        </section>
        <section id="medicine-management" class="page">
            <h2>Medicine Management</h2>
            <form id="add-medicine-form" class="content-box">
                <h3>Add New Medicine</h3>
                <label for="brand-name">Brand Name:</label>
                <input type="text" id="brand-name" placeholder="Enter brand name">
                <label for="generic-name">Generic Name:</label>
                <input type="text" id="generic-name" placeholder="Enter generic name">
                <label for="dosage">Dosage Strength:</label>
                <input type="text" id="dosage" placeholder="Enter dosage strength">
                <label for="packaging">Packaging Size:</label>
                <input type="text" id="packaging" placeholder="Enter packaging size">
                <label for="supplier">Supplier Information:</label>
                <input type="text" id="supplier" placeholder="Enter supplier information">
                <button type="button" onclick="addMedicine()">Add Medicine</button>
            </form>
            <form id="update-medicine-form" class="content-box">
                <h3>Update Medicine Information</h3>
                <!-- Similar structure as add-medicine-form -->
            </form>
        </section>
        <section id="stock-management" class="page">
            <h2>Stock Management</h2>
            <div class="stock-info">
                <label for="expiry-check">Check Expiry Dates:</label>
                <input type="text" id="expiry-check" placeholder="Enter medicine name">
                <button onclick="checkExpiry()">Check Expiry</button>
            </div>
            <div id="stock-alerts" class="content-box">
                <!-- Dynamic content will be loaded here -->
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Pharmacy Management System</p>
    </footer>
    <script src="scripts.js"></script>
</body>
</html>
