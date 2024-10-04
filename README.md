# Stock Trading Bot Application

    <h2>Overview</h2>
    <p>This is a backend application built with Node.js that simulates a basic trading bot for a hypothetical stock market. The bot continuously monitors stock price changes using mock data and executes trades based on predefined rules. It also tracks the bot's balance, shares owned, and profit/loss over time. The application logs trades and prints analytics in real-time.</p>

    <h2>Features</h2>
    <ul>
        <li><strong>Simulated Stock Prices</strong>: The application fetches mock stock prices in real-time.</li>
        <li><strong>Trading Logic</strong>: Implements a simple strategy:
            <ul>
                <li><strong>Buy</strong>: When the stock price drops by 2% from the last price.</li>
                <li><strong>Sell</strong>: When the stock price increases by 3% from the last price.</li>
            </ul>
        </li>
        <li><strong>Profit/Loss Tracking</strong>: Tracks the bot's current balance, shares owned, and overall profit/loss.</li>
        <li><strong>Logging</strong>: Trades and analytics are logged in both the terminal and a <code>tradeLog.txt</code> file.</li>
        <li><strong>Performance Analytics</strong>: Includes metrics for total trades, profit/loss ratio, and overall performance.</li>
    </ul>

    <h2>Technologies Used</h2>
    <ul>
        <li><strong>Node.js</strong>: Backend framework.</li>
        <li><strong>Express.js</strong>: Web server framework.</li>
        <li><strong>Mock API</strong>: Simulated stock prices via a custom mock API.</li>
        <li><strong>File System (fs)</strong>: For logging trades to a file.</li>
        <li><strong>Dotenv</strong>: For managing environment variables.</li>
    </ul>

    <h2>Getting Started</h2>

    <h3>Prerequisites</h3>
    <p>Node.js installed on your machine.</p>
    <p>A basic understanding of Node.js and Express.</p>

    <h3>Installation</h3>
    <ol>
        <li><strong>Clone the repository</strong>:
            <pre><code>git clone https://github.com/your-username/stock-trading-bot.git
cd stock-trading-bot</code></pre>
        </li>
        <li><strong>Install dependencies</strong>:
            <pre><code>npm install</code></pre>
        </li>
        <li><strong>Create <code>.env</code> file</strong>:
            <p>Create a <code>.env</code> file in the root directory to define the environment variables. Example:</p>
            <pre><code>PORT=3000</code></pre>
        </li>
        <li><strong>Run the application</strong>:
            <pre><code>npm start</code></pre>
            <p>The server will start running on <code>http://localhost:3000</code>.</p>
        </li>
    </ol>

    <h2>How It Works</h2>
    <ol>
        <li>The bot simulates stock prices every 5 seconds using a mock API.</li>
        <li>Based on the trading strategy:
            <ul>
                <li>The bot buys shares when the stock price drops by 2%.</li>
                <li>The bot sells shares when the stock price rises by 3%.</li>
            </ul>
        </li>
        <li>Each trade is logged in the <code>tradeLog.txt</code> file and displayed in the terminal.</li>
        <li>Performance metrics like total profit, loss, and number of trades are printed at the end of each session.</li>
    </ol>

    <h2>Endpoints</h2>
    <ul>
        <li><code>GET /</code>: Returns a message that the trading bot is running.</li>
    </ul>

    <h2>Example Output</h2>
    <pre><code>
Server is running on http://localhost:3000
Starting trading bot...
Current stock price: $55.24
No trade executed.
Current stock price: $49.99
Trade executed: Bought 200 shares at
