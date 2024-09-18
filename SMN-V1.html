
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Code Installer with Search and Delete</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2 {
            text-align: center;
            color: #333;
        }
        textarea {
            width: 100%;
            height: 150px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            padding: 10px;
            border-radius: 5px;
        }
        input[type="text"] {
            width: calc(100% - 120px);
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-right: 10px;
            margin-bottom: 10px;
        }
        button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
        .code-list {
            margin-top: 20px;
        }
        .code-item {
            padding: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #f9f9f9;
            margin-top: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .search-container {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>HTML Code Installer</h1>

        <!-- Search Bar -->
        <div class="search-container">
            <input type="text" id="searchBar" placeholder="Search code by name...">
            <button onclick="searchCode()">Search</button>
        </div>
        
        <label for="codeName">Code Name:</label>
        <input type="text" id="codeName" placeholder="Enter code name">

        <label for="htmlCode">Enter HTML Code:</label>
        <textarea id="htmlCode" placeholder="Write your HTML code here..."></textarea>

        <button class="install-button" onclick="installCode()">Install Code</button>

        <h2>Delete Installed Code</h2>
        <input type="text" id="deleteCodeName" placeholder="Enter code name to delete">
        <button class="delete-button" onclick="deleteCode()">Delete Code</button>

        <div class="code-list">
            <h2>Installed Codes</h2>
            <div id="installedCodes"></div>
        </div>
    </div>

    <script>
        let installedCodes = [];

        // Load codes from localStorage on page load
        window.onload = function() {
            const savedCodes = localStorage.getItem('installedCodes');
            if (savedCodes) {
                installedCodes = JSON.parse(savedCodes);
                displayInstalledCodes();
            }
        };

        function installCode() {
            const codeName = document.getElementById('codeName').value;
            const htmlCode = document.getElementById('htmlCode').value;

            if (codeName && htmlCode) {
                // Add the new code to the list of installed codes
                installedCodes.push({ name: codeName, code: htmlCode });

                // Save the updated list to localStorage
                localStorage.setItem('installedCodes', JSON.stringify(installedCodes));

                // Show the list of installed codes
                displayInstalledCodes();

                // Clear the input fields
                document.getElementById('codeName').value = '';
                document.getElementById('htmlCode').value = '';
            } else {
                alert('Please enter both a code name and HTML code.');
            }
        }

        function displayInstalledCodes(codes = installedCodes) {
            const installedCodesDiv = document.getElementById('installedCodes');
            installedCodesDiv.innerHTML = '';

            codes.forEach((item, index) => {
                const codeItem = document.createElement('div');
                codeItem.classList.add('code-item');

                codeItem.innerHTML = `
                    <h3>${item.name}</h3>
                    <button onclick="useCode(${index})">Use Code</button>
                `;

                installedCodesDiv.appendChild(codeItem);
            });
        }

        function useCode(index) {
            const codeItem = installedCodes[index];
            const previewWindow = window.open();
            previewWindow.document.write(codeItem.code);
        }

        function deleteCode() {
            const deleteCodeName = document.getElementById('deleteCodeName').value;

            if (deleteCodeName) {
                // Find the index of the code to be deleted
                const codeIndex = installedCodes.findIndex(item => item.name === deleteCodeName);

                if (codeIndex !== -1) {
                    // Remove the code from the array
                    installedCodes.splice(codeIndex, 1);

                    // Update localStorage with the new list
                    localStorage.setItem('installedCodes', JSON.stringify(installedCodes));

                    // Update the displayed list of installed codes
                    displayInstalledCodes();

                    // Clear the delete input field
                    document.getElementById('deleteCodeName').value = '';
                } else {
                    alert('Code name not found!');
                }
            } else {
                alert('Please enter a code name to delete.');
            }
        }

        // Search function for codes by name
        function searchCode() {
            const searchTerm = document.getElementById('searchBar').value.toLowerCase();

            // Filter the installed codes by name
            const filteredCodes = installedCodes.filter(item => 
                item.name.toLowerCase().includes(searchTerm)
            );

            // Display the filtered codes
            displayInstalledCodes(filteredCodes);
        }
    </script>

</body>
</html>
