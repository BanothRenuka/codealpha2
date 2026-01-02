<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rule-Based Chatbot</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            padding: 20px;
        }
        
        .container {
            width: 100%;
            max-width: 800px;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(to right, #2575fc, #6a11cb);
            color: white;
            padding: 20px;
            text-align: center;
        }
        
        h1 {
            font-size: 28px;
            margin-bottom: 5px;
        }
        
        .subtitle {
            font-size: 16px;
            opacity: 0.9;
        }
        
        .chat-container {
            display: flex;
            flex-direction: column;
            height: 500px;
            padding: 20px;
        }
        
        .chat-history {
            flex: 1;
            overflow-y: auto;
            padding: 15px;
            border: 1px solid #e0e0e0;
            border-radius: 10px;
            margin-bottom: 20px;
            background-color: #f9f9f9;
        }
        
        .message {
            margin-bottom: 15px;
            max-width: 80%;
            clear: both;
        }
        
        .user-message {
            float: right;
            background-color: #2575fc;
            color: white;
            border-radius: 15px 15px 0 15px;
            padding: 10px 15px;
        }
        
        .bot-message {
            float: left;
            background-color: #e9e9e9;
            color: #333;
            border-radius: 15px 15px 15px 0;
            padding: 10px 15px;
        }
        
        .message-sender {
            font-size: 12px;
            margin-bottom: 3px;
            font-weight: bold;
        }
        
        .user-message .message-sender {
            text-align: right;
            color: #1c5fd6;
        }
        
        .bot-message .message-sender {
            text-align: left;
            color: #6a11cb;
        }
        
        .input-area {
            display: flex;
            gap: 10px;
        }
        
        input {
            flex: 1;
            padding: 12px 15px;
            border: 2px solid #ddd;
            border-radius: 25px;
            font-size: 16px;
            outline: none;
            transition: border-color 0.3s;
        }
        
        input:focus {
            border-color: #6a11cb;
        }
        
        button {
            background: linear-gradient(to right, #2575fc, #6a11cb);
            color: white;
            border: none;
            border-radius: 25px;
            padding: 0 25px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
        }
        
        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
        }
        
        button:active {
            transform: translateY(0);
        }
        
        .suggestions {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        
        .suggestion-btn {
            background-color: #f0f0f0;
            color: #333;
            border: none;
            border-radius: 20px;
            padding: 8px 15px;
            font-size: 14px;
            cursor: pointer;
            transition: background-color 0.2s;
        }
        
        .suggestion-btn:hover {
            background-color: #e0e0e0;
        }
        
        .info-panel {
            background-color: #f5f7ff;
            border-top: 1px solid #e0e0e0;
            padding: 15px 20px;
            font-size: 14px;
            color: #555;
        }
        
        .info-panel h3 {
            margin-bottom: 10px;
            color: #6a11cb;
        }
        
        .rules-list {
            columns: 2;
            list-style-type: none;
        }
        
        .rules-list li {
            margin-bottom: 8px;
            padding-left: 20px;
            position: relative;
        }
        
        .rules-list li:before {
            content: "•";
            color: #2575fc;
            font-weight: bold;
            position: absolute;
            left: 0;
        }
        
        @media (max-width: 768px) {
            .rules-list {
                columns: 1;
            }
            
            .chat-container {
                height: 400px;
            }
        }
        
        .clear-btn {
            background: linear-gradient(to right, #ff416c, #ff4b2b);
            margin-top: 10px;
            padding: 8px 15px;
            font-size: 14px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Rule-Based Chatbot</h1>
            <div class="subtitle">Responds to: "hello", "how are you", "bye", and more!</div>
        </header>
        
        <div class="chat-container">
            <div class="chat-history" id="chatHistory">
                <!-- Chat messages will appear here -->
                <div class="message bot-message">
                    <div class="message-sender">Chatbot</div>
                    <div>Hello! I'm a simple rule-based chatbot. Try saying "hello", "how are you", or "bye".</div>
                </div>
            </div>
            
            <div class="input-area">
                <input type="text" id="userInput" placeholder="Type your message here..." autocomplete="off">
                <button id="sendBtn">Send</button>
            </div>
            
            <div class="suggestions">
                <button class="suggestion-btn" data-message="hello">Hello</button>
                <button class="suggestion-btn" data-message="how are you">How are you?</button>
                <button class="suggestion-btn" data-message="what is your name">What's your name?</button>
                <button class="suggestion-btn" data-message="bye">Goodbye</button>
                <button class="suggestion-btn" data-message="help">Help</button>
                <button class="suggestion-btn clear-btn" id="clearBtn">Clear Chat</button>
            </div>
        </div>
        
        <div class="info-panel">
            <h3>How This Chatbot Works</h3>
            <ul class="rules-list">
                <li>Uses if-elif conditional logic to match user input</li>
                <li>Predefined responses for specific phrases</li>
                <li>Case-insensitive matching (try "Hello" or "HELLO")</li>
                <li>Input/output handled through JavaScript functions</li>
                <li>Chat loop continues until page refresh</li>
                <li>Try: "hello", "how are you", "what is your name", "bye", "help"</li>
            </ul>
        </div>
    </div>

    <script>
        // DOM elements
        const chatHistory = document.getElementById('chatHistory');
        const userInput = document.getElementById('userInput');
        const sendBtn = document.getElementById('sendBtn');
        const clearBtn = document.getElementById('clearBtn');
        const suggestionBtns = document.querySelectorAll('.suggestion-btn');
        
        // Predefined responses for the chatbot
        function getBotResponse(userMessage) {
            // Convert to lowercase for case-insensitive matching
            const message = userMessage.toLowerCase().trim();
            
            // Rule-based responses using if-elif logic
            if (message.includes('hello') || message.includes('hi') || message.includes('hey')) {
                return "Hi there! How can I help you today?";
            } 
            else if (message.includes('how are you')) {
                return "I'm doing great, thanks for asking! How about you?";
            } 
            else if (message.includes('what is your name') || message.includes('your name')) {
                return "I'm a simple rule-based chatbot created with HTML, CSS, and JavaScript!";
            } 
            else if (message.includes('bye') || message.includes('goodbye') || message.includes('see you')) {
                return "Goodbye! Have a wonderful day!";
            } 
            else if (message.includes('help')) {
                return "I'm a simple chatbot that responds to basic phrases. Try saying: hello, how are you, what is your name, or bye.";
            }
            else if (message.includes('thank')) {
                return "You're welcome! I'm glad I could help.";
            }
            else if (message.includes('weather')) {
                return "I'm just a simple chatbot and don't have access to weather data. But I hope it's nice where you are!";
            }
            else if (message.includes('time') || message.includes('date')) {
                const now = new Date();
                return `The current date and time is: ${now.toLocaleString()}`;
            }
            else {
                return "I'm sorry, I don't understand that. I'm a simple rule-based chatbot. Try saying hello, how are you, or bye.";
            }
        }
        
        // Function to add a message to the chat history
        function addMessage(sender, message) {
            const messageDiv = document.createElement('div');
            messageDiv.className = `message ${sender}-message`;
            
            const senderDiv = document.createElement('div');
            senderDiv.className = 'message-sender';
            senderDiv.textContent = sender === 'user' ? 'You' : 'Chatbot';
            
            const messageContent = document.createElement('div');
            messageContent.textContent = message;
            
            messageDiv.appendChild(senderDiv);
            messageDiv.appendChild(messageContent);
            
            chatHistory.appendChild(messageDiv);
            
            // Scroll to the bottom of the chat history
            chatHistory.scrollTop = chatHistory.scrollHeight;
        }
        
        // Function to handle user input
        function handleUserInput() {
            const message = userInput.value.trim();
            
            if (message === '') return;
            
            // Add user message to chat
            addMessage('user', message);
            
            // Get bot response
            const botResponse = getBotResponse(message);
            
            // Simulate a small delay before bot responds (more natural)
            setTimeout(() => {
                addMessage('bot', botResponse);
            }, 500);
            
            // Clear input field
            userInput.value = '';
            userInput.focus();
        }
        
        // Event Listeners
        sendBtn.addEventListener('click', handleUserInput);
        
        userInput.addEventListener('keypress', (e) => {
            if (e.key === 'Enter') {
                handleUserInput();
            }
        });
        
        clearBtn.addEventListener('click', () => {
            // Clear chat history except the first bot message
            const initialMessage = chatHistory.querySelector('.bot-message');
            chatHistory.innerHTML = '';
            chatHistory.appendChild(initialMessage);
        });
        
        // Add event listeners to suggestion buttons
        suggestionBtns.forEach(btn => {
            if (btn.id !== 'clearBtn') {
                btn.addEventListener('click', () => {
                    const message = btn.getAttribute('data-message');
                    userInput.value = message;
                    handleUserInput();
                });
            }
        });
        
        // Add initial greeting
        window.addEventListener('load', () => {
            userInput.focus();
        });
    </script>
</body>
</html>