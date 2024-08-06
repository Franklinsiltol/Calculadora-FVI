<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora de Taxas</title>
</head>
<body>
    <h2>Calculadora de Taxas</h2>
    <form id="taxCalculator">
        <label for="transactionValue">Valor da Transação (R$):</label>
        <input type="number" id="transactionValue" name="transactionValue" step="0.01" required><br><br>
        
        <label for="sumUpRate">Taxa SumUp (%):</label>
        <input type="number" id="sumUpRate" name="sumUpRate" step="0.01" required><br><br>
        
        <label for="competitorRate">Taxa da Concorrente (%):</label>
        <input type="number" id="competitorRate" name="competitorRate" step="0.01" required><br><br>
        
        <button type="button" onclick="calculate()">Calcular</button>
    </form>
    
    <h3>Resultados:</h3>
    <p id="sumUpValue">Valor a receber com a taxa SumUp: R$</p>
    <p id="competitorValue">Valor a receber com a taxa da concorrente: R$</p>
    <p id="difference">Diferença: R$</p>

    <script>
        function calculate() {
            // Obtém os valores do formulário
            let transactionValue = parseFloat(document.getElementById('transactionValue').value);
            let sumUpRate = parseFloat(document.getElementById('sumUpRate').value);
            let competitorRate = parseFloat(document.getElementById('competitorRate').value);
            
            // Calcula os valores a receber
            let sumUpValue = transactionValue * (1 - sumUpRate / 100);
            let competitorValue = transactionValue * (1 - competitorRate / 100);
            
            // Calcula a diferença
            let difference = sumUpValue - competitorValue;
            
            // Atualiza os resultados no HTML
            document.getElementById('sumUpValue').innerText = `Valor a receber com a taxa SumUp: R$ ${sumUpValue.toFixed(2)}`;
            document.getElementById('competitorValue').innerText = `Valor a receber com a taxa da concorrente: R$ ${competitorValue.toFixed(2)}`;
            document.getElementById('difference').innerText = `Diferença: R$ ${difference.toFixed(2)}`;
        }
    </script>
</body>
</html>
