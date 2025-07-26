# Rain Alert

This project is a Python script that checks the weather forecast for a specific location and sends an SMS notification if it is going to rain within the next 12 hours.

## Features

- Fetches weather data from the OpenWeatherMap API.
- Sends an SMS notification using the Twilio API.
- Uses environment variables to keep API keys and other sensitive information secure.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Python 3.x
- A Twilio account
- An OpenWeatherMap API key

### Installation

1.  Clone the repository:
    ```bash
    git clone <repository-url>
    ```
2.  Navigate to the project directory:
    ```bash
    cd rain_alert
    ```
3.  Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Configuration

1.  Create a `.env` file in the root of the project.
2.  Add your API keys and phone numbers to the `.env` file:

    ```
    OWM_api_key="YOUR_OPENWEATHERMAP_API_KEY"
    twilio_account_sid="YOUR_TWILIO_ACCOUNT_SID"
    twilio_auth_token="YOUR_TWILIO_AUTH_TOKEN"
    from_phone="YOUR_TWILIO_VIRTUAL_NUMBER"
    to_phone="YOUR_TWILIO_VERIFIED_REAL_NUMBER"
    ```

## Usage

Run the `main.py` script to check the weather and send a notification if rain is forecasted.

```bash
python main.py
```