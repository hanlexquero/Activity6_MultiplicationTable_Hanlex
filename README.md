<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
</head>
<body>
    <script>
        var num = prompt("Enter a number:");
        let table = document.createElement("table");
        document.write("<table border= 1>");
            
        for (let a = num; a >= 1; a--) {
          let row = document.createElement("tr");
          for (let b = num; b >= 1; b--) {
            let cell = document.createElement("td");

            let value = a * b;

            cell.textContent = value;

            row.appendChild(cell);

            if (a === 1 && b === 1) {
              cell.style.backgroundColor = "yellow";
            }

            if (a === 1 && b === num) {
              cell.style.backgroundColor = "yellow";
            }
            if (a === num && b=== 1) {
              cell.style.backgroundColor = "yellow";
            }
            if (a === num && b === num) {
              cell.style.backgroundColor = "yellow";
            }
          }
          table.appendChild(row);
        }
        document.body.appendChild(table);
    </script>
</body>
</html>
