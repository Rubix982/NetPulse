# NetPulse  

**NetPulse** is a lightweight tool that periodically measures your internet speed using a cron job and stores the results locally. You can view the logged data either via the command-line interface or in your browser, ensuring you always have a clear view of your internet performance history.

## Features

- **Automated Testing**: Runs speed tests periodically via cron jobs.  
- **Local Data Storage**: Saves speed test results locally for privacy and easy access.  
- **Multi-Platform Viewing**:  
  - **CLI**: Access results directly from the terminal.  
  - **Browser**: View a simple, user-friendly dashboard for insights.  
- **Customizable**: Adjust test frequency and storage paths to fit your needs.  

## Getting Started  

### Prerequisites  

> TODO: This section needs to be updated

- **Node.js** or **Python** (depending on the implementation).  
- [Speedtest CLI](https://www.speedtest.net/apps/cli) or a similar speed test tool.  
- A basic web server (e.g., Python's built-in HTTP server or Node.js' `http-server`).

### Installation

> TODO: This section needs to be updated

1. Clone the repository,

 ```bash
git clone https://github.com/yourusername/SpeedChronicle.git
cd SpeedChronicle
```

2. Install dependencies:

```sh
# For Node.js (if applicable)
npm install  

# For Python (if applicable)
pip install -r requirements.txt  
```

3. Set up the cron job,
  - Open your crontab,

```sh
crontab -e
```

  - Add an entry to run the speed test script periodically. For example, to run every hour,

```text
0 * * * * /path/to/speed_test_script >> /path/to/logfile.json
```

4. Start the local web server (optional):

```sh
# For Python
python -m http.server  

# For Node.js
npx http-server
```

## Usage

### Command-Line Interface

> TODO: This section needs to be updated

Run the following to view results in the terminal:

python speedchronicle_cli.py  # or
node speedchronicle_cli.js

### Browser Dashboard

1. Open the browser and go to http://localhost:8000 (adjust port if needed).
2. Browse through historical speed test data with easy-to-read charts and logs.

## Customization

•	Test Frequency: Edit your cron job to adjust the interval (e.g., daily, hourly).
•	Storage Path: Configure the file path for storing results in the .env file or script settings.
•	Output Format: Results can be stored in JSON or CSV format, depending on your preference.

## License

This project is licensed under the MIT License.

## Feedback

Feel free to open an issue for bugs, suggestions, or feature requests!
