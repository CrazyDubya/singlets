# Negotiation Chatbot

This repository contains a simple web-based negotiation chatbot.

## Description

The `chat_negotiate.html` file implements a chatbot that simulates a price negotiation with a user. The chatbot starts with an initial price for an item and engages in a conversation with the user to agree on a final price.

## How to Use

1.  Clone or download this repository.
2.  Open the `chat_negotiate.html` file in a web browser.
3.  The chat interface will load, and the bot will make an initial offer.
4.  Enter your counter-offers in the input field and click "Send".
5.  The bot will respond based on its negotiation logic until a deal is made or the conversation reaches a stalemate based on its programmed rules.

## Negotiation Logic

-   **Base Price**: The bot operates with a predefined base price for the item (e.g., $100).
-   **Initial Offer**: The bot starts the negotiation by offering a price that is a certain percentage higher than the base price (e.g., 20% markup).
-   **Acceptable Discount**: The bot is programmed with a minimum and maximum acceptable discount range (e.g., 18-22% off the base price). If the user's offer falls within this range, the bot will accept it.
-   **Counter-Offers**: If the user's offer is too low (below the minimum acceptable discount), the bot will make a counter-offer or use "hardball" tactics. It tries to progressively get closer to a mutually agreeable price.
-   **Communication Style**: The bot uses a variety of phrases for different situations (making initial offers, responding to low offers, accepting deals, etc.) to make the interaction feel more dynamic.

This is a simple client-side application written in HTML and JavaScript. All the logic is contained within the `chat_negotiate.html` file.

## Running Tests

Automated tests for the JavaScript logic are available in `test_runner.html`.
To run the tests:
1.  Open `test_runner.html` in your web browser.
2.  The page will display the test results, indicating how many tests passed or failed.
3.  Check the browser's developer console for more detailed error messages if any tests fail.