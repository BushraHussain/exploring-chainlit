##Steps to integrate FastAPI:
1. Create a new uv project by running `uv init integrations`
2. "uv venv" for creating a virtual environment. Activate it by running `source .venv/bin/activate`
3. Install Chainlit by running `uv add chainlit` and FastAPI by running `uv add fastapi`
4. Run "uv run chainlit hello" to ensure it's working
5. When we install chainlit, it creates a hello.py file. This is the entrypoint for our app. 
6. Let's delete it and create a new file named "chatbot.py" and write main function with decorator @cl.on_chat_start
7. Make another file named "main.py" and write a simple FastAPI app with mount_chainlit function
8. Now run "uv run uvicorn main:app --host 0.0.0.0 --port 80" to start the app. 
8. Now go to http://0.0.0.0/app to see the fastapi endpoint
9. And go to http://0.0.0.0/chainlit to see the chatbot

For more details: https://docs.chainlit.io/integrations/fastapi

##Steps to integrate OpenAi:
1. Install openai by running "uv add openai"
2. Create a .env file in the root directory and add your openai key e.g. OPENAI_API_KEY=key_here
3. Make a new file in the root directory named "openai_integration.py" and add the code
4. Run the file using the command "chainlit run openai_integration.py -w"

For more details: https://docs.chainlit.io/integrations/openai