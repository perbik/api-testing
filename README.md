# Restful-Booker API Automation Testing

## Project Overview

This project contains an automated API test suite developed using Postman for the Restful-Booker API.

The objective is to validate the booking lifecycle, including authentication, booking creation, updating, verification, and deletion. It also includes negative testing to verify that unauthorized requests are properly rejected.

**API Base URL:** https://restful-booker.herokuapp.com

## Tools and Technologies

- Postman
- JavaScript

## Test Coverage

| No. | Request | Method | Purpose |
|---|---|---|---|
| 1 | Create Auth Token | POST | Generate authentication token |
| 2 | Create Booking | POST | Create booking and extract booking ID |
| 3 | Update Booking | PUT | Update booking using dynamic ID and token |
| 4 | Update Booking - Invalid Token | PUT | Verify unauthorized update is rejected |
| 5 | Verify Booking | GET | Validate updated booking information |
| 6 | Delete Booking | DELETE | Delete test booking |

## Environment Variables

| Variable | Description |
|---|---|
| baseUrl | Restful-Booker API base URL |
| token | Dynamically generated authentication token |
| bookingId | Dynamically generated booking ID |

## How to Run

1. Download or clone this repository.
2. Open Postman.
3. Import the exported Postman collection JSON file.
4. Create or import the Restful-Booker environment template.
5. Select the environment.
6. Open the Collection Runner.
7. Execute all requests in their defined order.
8. Review the test results.

The authentication token and booking ID are automatically generated and stored during execution.

## Expected Results

All automated assertions should pass when the API responds as expected.

## Repository Contents

- `Restful-Booker-API-Test-Suite.postman_collection.json` - Exported Postman collection.
- `Restful-Booker-Environment.postman_environment.json` - Environment template.
