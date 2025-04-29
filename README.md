# ShopFast Customer Support Assistant

A lightweight conversational AI agent for e-commerce customer support, built using pretrained local models.

## Features

- Intent Recognition using DistilBERT
- Context-aware responses
- Simple chat interface using Streamlit
- Support for 6 predefined intents:
  - Order Tracking
  - Return & Refund Policy
  - Product Availability
  - Store Location/Hours
  - General Greetings
  - Unknown/Other

## Installation

1. Clone this repository
2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the Streamlit app:
```bash
streamlit run app.py
```

2. Open your web browser and navigate to the URL shown in the terminal (usually http://localhost:8501)

3. Start chatting with the assistant!

## Model Architecture

- Base Model: DistilBERT (distilbert-base-uncased)
- Fine-tuned for intent classification
- Uses a simple rule-based response system
- Implements basic context handling for product-related queries

## Sample Conversations

1. Order Tracking:
```
User: Where is my order?
Assistant: Please share your order ID to help track your package.
```

2. Product Availability with Context:
```
User: Do you have Nike shoes in stock?
Assistant: Regarding nike, I can help you check product availability. Which item are you looking for?
```

3. Store Hours:
```
User: What are your store hours?
Assistant: Our stores are open Monday-Saturday, 9 AM to 9 PM. Would you like to find the nearest store?
```

![WhatsApp Image 2025-04-29 at 23 00 59_9235d44a](https://github.com/user-attachments/assets/751b9dff-c935-4b95-b7d6-4cc0289a1a51)
![WhatsApp Image 2025-04-29 at 23 01 26_0e3d877f](https://github.com/user-attachments/assets/156c6bab-edfc-4efb-96e2-c8632cbaf560)
![WhatsApp Image 2025-04-29 at 23 01 47_0545530f](https://github.com/user-attachments/assets/992a5928-eacc-49b0-ba77-39f7bd0f3635)

## Libraries Used

- transformers: For the DistilBERT model
- torch: For deep learning operations
- pandas: For data handling
- scikit-learn: For data preprocessing and model evaluation
- streamlit: For the web interface
- numpy: For numerical operations

## Limitations

- Limited to predefined intents
- Basic context handling
- No persistent storage
- Limited training data

## Future Improvements

- Add more training data
- Implement more sophisticated context handling
- Add product search functionality
- Improve response generation
- Add confidence score display
- Implement multi-turn conversation handling 

