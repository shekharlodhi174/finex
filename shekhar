<script>
    async function fetchMarketData() {
        const apiKey = 'YOUR_API_KEY'; // Alpha Vantage se free API key lein
        const url = `https://www.alphavantage.co/query?function=INDEX_QUOTE&symbol=NIFTY%2050&apikey=${apiKey}`;
        try {
            const response = await fetch(url);
            const data = await response.json();
            // Update table with data
            document.getElementById('nifty-value').innerText = data['index_quote']['05. price'];
            document.getElementById('nifty-change').innerText = data['index_quote']['09. change'];
            document.getElementById('nifty-percent').innerText = data['index_quote']['10. change_percent'];
        } catch (error) {
            console.error('Error fetching data:', error);
        }
    }
    fetchMarketData();
</script>
