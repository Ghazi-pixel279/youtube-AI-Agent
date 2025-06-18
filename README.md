# youtube-AI-Agentfrom flask import Flask

app = Flask(_name_)

@app.route('/')
def home():
    return "YouTube AI Agent is Running!"

if _name_ == '_main_':
    app.run(host='0.0.0.0', port=10000) services:
  - type: web
    name: youtube-ai-agent
    env: python
    buildCommand: ""
    startCommand: "python main.py"
    plan: free
