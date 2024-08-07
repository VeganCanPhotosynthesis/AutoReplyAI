# AutoReplyAI

AutoReplyAI is a project designed to automate email responses using OpenAI's GPT-3.5-turbo model. It identifies auto-reply messages and generates tailored responses based on specific scenarios, ensuring efficient and personalized communication with leads.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Scenarios](#scenarios)


## Installation

To set up this project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://gitlab.com/your-username/your-repository.git
    ```
2. Navigate to the project directory:
    ```sh
    cd your-repository
    ```
3. Install the required dependencies:
    ```sh
    pip install openai
    ```

## Usage

1. Set your OpenAI API key by replacing `your-api-key` in the notebook:
    ```python
    openai.api_key = 'your-api-key'
    ```
2. Open the Jupyter notebook:
    ```sh
    jupyter notebook
    ```
3. Define the reply data and the required variables such as `name`, `company_name`, `product`, `value`, `pains`, `solutions`, `stories`, `trust`, `objections`, and `CalendarLink` within the notebook cells.

4. Run the notebook cells to generate email responses.

## Configuration

The notebook uses two main API calls to OpenAI's GPT-3.5-turbo model:

1. **Initial Response Generation**: 
    - Checks if the email is an auto-reply.
    - If not an auto-reply, generates a draft response based on the provided scenarios.

2. **Response Refinement**: 
    - Modifies the draft response to include necessary details and ensures conciseness.

### Variables

- `reply_data`: The content of the email to respond to.
- `name`: Your name as the Sales Development Representative.
- `company_name`: The name of your company.
- `product`: Details about the product.
- `value`: Value proposition of the product.
- `pains`: Pain points addressed by the product.
- `solutions`: Solutions provided by the product.
- `stories`: Customer stories or testimonials.
- `trust`: Elements that build trust.
- `objections`: Common objections and responses.
- `CalendarLink`: Direct link to a calendar tool for scheduling meetings.

## Scenarios

The following scenarios are handled by the script:

- **Scheduling a Call**
- **Providing Product Information**
- **Following Up for a Proof of Concept (POC)**
- **Re-engaging Interest**
- **Handling Non-Interest Responses**

Each scenario involves crafting personalized responses that address the specific needs and concerns of the lead.

