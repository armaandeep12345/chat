<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ChatBot</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f8ff;
            font-family: Arial, sans-serif;
        }

        .chatbox {
            width: 320px;
            height: 550px;
            background: linear-gradient(135deg, #6e7bff, #9b3eff);
            border-radius: 15px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
            display: flex;
            flex-direction: column;
            overflow: hidden;
        }

        .header {
            padding: 18px;
            background-color: #4c6bff;
            color: white;
            font-weight: bold;
            text-align: center;
            border-radius: 15px 15px 0 0;
            font-size: 1.2rem;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .chat-content {
            flex: 1;
            padding: 15px;
            overflow-y: auto;
            background-color: #f9f9f9;
            border-radius: 10px;
        }

        .message {
            display: flex;
            align-items: center;
            margin: 8px 0;
        }

        .message.bot {
            flex-direction: row;
        }

        .message.user {
            flex-direction: row-reverse;
        }

        .avatar {
            font-size: 30px;
            color: #fff;
            display: flex;
            align-items: center;
            justify-content: center;
            width: 35px;
            height: 35px;
            border-radius: 50%;
        }

        .bot-avatar {
            background-color: #5a5aff;
        }

        .user-avatar {
            background-color: #ff7043;
        }

        .text {
            padding: 12px;
            border-radius: 10px;
            margin: 0 12px;
            max-width: 75%;
            background-color: #e0e0e0;
            box-shadow: 0 3px 6px rgba(0, 0, 0, 0.1);
            white-space: pre-wrap;
        }

        .user .text {
            background-color: #ffeb3b;
        }

        .time {
            font-size: 10px;
            color: #888;
        }

        .choices {
            display: flex;
            flex-direction: column;
            gap: 8px;
            margin: 10px 0;
        }

        .choices button {
            background-color: #5a5aff;
            border: none;
            padding: 10px;
            border-radius: 8px;
            color: white;
            cursor: pointer;
            font-size: 0.9rem;
        }

        .choices button:hover {
            background-color: #4c6bff;
        }

        .input-area {
            display: flex;
            padding: 12px;
            background-color: #fff;
            border-top: 2px solid #ddd;
            box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.1);
        }

        input[type="text"] {
            flex: 1;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 8px;
            outline: none;
        }

        button {
            background-color: #5a5aff;
            border: none;
            padding: 12px 18px;
            margin-left: 10px;
            border-radius: 8px;
            color: white;
            cursor: pointer;
        }

        button:hover {
            background-color: #4c6bff;
        }
    </style>
</head>
<body>
    <div class="chatbox">
        <div class="header">ChatBot</div>
        <div class="chat-content"></div>
        <div class="input-area">
            <input type="text" placeholder="Type your message..." aria-label="Type your message">
            <button aria-label="Send message">Send</button>
        </div>
    </div>

    <script>
        const button = document.querySelector("button");
        const input = document.querySelector("input[type='text']");
        const chatContent = document.querySelector(".chat-content");

        window.onload = () => {
            addMessage("bot", "Hi there! 👋 Techcadd Computer Education pvt. ltd. Type 'list of courses' to get started!");
        };

        button.addEventListener("click", sendMessage);
        input.addEventListener("keydown", (event) => {
            if (event.key === "Enter") sendMessage();
        });

        function sendMessage() {
            const userMessage = input.value.trim();
            if (userMessage) {
                addMessage("user", userMessage);
                input.value = "";

                setTimeout(() => {
                    const reply = generateReply(userMessage);
                    if (reply.type === "text") {
                        addMessage("bot", reply.text);
                    } else if (reply.type === "choices") {
                        addChoices(reply.choices);
                    }
                }, 1000);
            } else {
                alert("Please enter a message!");
            }
        }

        function addMessage(sender, text) {
            const messageDiv = document.createElement("div");
            messageDiv.className = `message ${sender}`;

            const avatarDiv = document.createElement("div");
            avatarDiv.className = `avatar ${sender}-avatar`;
            const icon = document.createElement("i");
            icon.className = sender === "bot" ? "fas fa-robot" : "fas fa-user";
            avatarDiv.appendChild(icon);

            const textDiv = document.createElement("div");
            textDiv.className = "text";
            textDiv.textContent = text;

            messageDiv.appendChild(avatarDiv);
            messageDiv.appendChild(textDiv);

            chatContent.appendChild(messageDiv);
            chatContent.scrollTo({ top: chatContent.scrollHeight, behavior: 'smooth' });
        }

        function addChoices(choices) {
            const choiceContainer = document.createElement("div");
            choiceContainer.className = "choices";

            choices.forEach(choice => {
                const button = document.createElement("button");
                button.textContent = choice;
                button.onclick = () => {
                    addMessage("user", choice);
                    const reply = generateReply(choice.toLowerCase());
                    setTimeout(() => {
                        addMessage("bot", reply.text);
                    }, 1000);
                };
                choiceContainer.appendChild(button);
            });

            chatContent.appendChild(choiceContainer);
            chatContent.scrollTo({ top: chatContent.scrollHeight, behavior: 'smooth' });
        }

        function generateReply(userMessage) {
    const message = userMessage.toLowerCase();
    if (message.includes("list of courses")) {
        return {
            type: "choices",
            choices: [
                "📚 Basic Computer Course",
                "📈 Digital Marketing Course",
                "🏗️ Civil/Architecture/Mechanical Courses",
                "💻 Advanced Computer Courses"
            ]
        };
    } else if (message.includes("basic computer")) {
        return { 
            type: "text", 
            text: "📚 Basic Computer Course:\n- 💻 Introduction to Computers\n- 📝 Notepad\n- 🖊️ WordPad\n- 🖥️ Microsoft Office (Word, Excel, PowerPoint)\n- 🌐 Internet Basics\n- 📧 Email Communication" 
        };
    } else if (message.includes("digital marketing")) {
        return { 
            type: "text", 
            text: "📈 Digital Marketing Course:\n- 📱 Social Media Marketing\n- 💻 Google Ads\n- 🔍 SEO Basics\n- ✍️ Content Marketing" 
        };
    } else if (message.includes("civil") || message.includes("architecture") || message.includes("mechanical")) {
        return { 
            type: "text", 
            text: "🏗️ Civil/Architecture/Mechanical Courses:\n- 📐 AutoCAD 2D & 3D\n- 🏢 Revit Architecture\n- 🔧 STAAD Pro\n- ⚙️ SolidWorks" 
        };
    } else if (message.includes("advanced computer")) {
        return { 
            type: "text", 
            text: "💻 Advanced Computer Courses:\n- 🐍 Python Programming\n- ☕ Java\n- ⚛️ React\n- 🌐 Node.js\n- 🌍 Web Development\n- 🛡️ Networking and Cybersecurity\n- 💻 C, C++ Programming\n- 🌐 Web Designing\n- 📱 Kotlin\n- 🔄 MEAN & MERN Stack\n- 🖥️ PHP Full Stack\n- 🤖 Artificial Intelligence\n- 📊 Power BI\n- 📈 Tableau\n- 📚 Data Science\n- 📊 Data Analytics\n- 🧠 Machine Learning\n- 🤖 Deep Learning" 
        };
    } else {
        return { 
            type: "text", 
            text: "I’m sorry, I didn’t understand that. Type 'list of courses' to see available options!" 
        };
    }
}

    </script>
</body>
</html>
