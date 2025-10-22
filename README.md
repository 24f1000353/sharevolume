# SEC Entity Common Stock Shares Outstanding Viewer

This project provides a single-page responsive web application to display the maximum and minimum common stock shares outstanding for a given company, fetched directly from the SEC EDGAR API. The application dynamically updates its content based on the Company Identification Key (CIK) provided in the URL or defaults to Ametek (AME) if no CIK is specified.

## Features

*   **Dynamic Data Fetching:** Retrieves `EntityCommonStockSharesOutstanding` data from the SEC EDGAR API.
*   **CIK-driven Content:** Easily view data for different companies by changing the CIK in the URL.
*   **Max/Min Shares Outstanding:** Highlights the highest and lowest reported shares outstanding since fiscal year 2021.
*   **Responsive Design:** Built with Tailwind CSS for a seamless experience across various devices.
*   **Error Handling:** Basic error handling for API requests.

## Setup

This is a single-file HTML application. No build steps or complex configurations are required.

1.  Save the `index.html` file to your local machine.
2.  Open `index.html` in any modern web browser.

## Usage

### Default View (Ametek)

To view the data for Ametek (CIK: 0001037868), simply open the `index.html` file:

`file:///path/to/your/folder/index.html`

### Custom CIK View

To view data for a different company, append a `?CIK=<your-cik-number>` query parameter to the URL. The CIK must be a 10-digit number (leading zeros are important).

Example for Tesla (CIK: 0001318605):

`file:///path/to/your/folder/index.html?CIK=0001318605`

The application will automatically fetch and display the relevant data without requiring a page reload.

## Data Source

All financial data is sourced from the [SEC EDGAR API](https://www.sec.gov/edgar/sec-api-documentation).

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
