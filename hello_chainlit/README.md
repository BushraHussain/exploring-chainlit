steps:
1. Create a new uv project by running `uv init hello_chainlit`
2. "uv venv" for creating a virtual environment. Activate it by running `source .venv/bin/activate`
3. Install Chainlit by running `uv add chainlit`
4. Run "uv run chainlit hello" to ensure it's working
5. When we install chainlit, it creates a hello.py file. This is the entrypoint for our app. 
6. Let's delete it and create a new file named "chatbot.py" 
7. Now run "uv run chainlit run chatbot.py -w" to start the chatbot. 
Note: the -w parameter enables hot reloading when we change our code
8. Now go to http://localhost:8000 to see the chatbot in action.

