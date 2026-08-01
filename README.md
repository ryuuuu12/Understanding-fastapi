* **Media Storage:** ImageKit

## Prerequisites
* Python >= 3.14

## Installation
1. Clone the repository.
2. Install the required dependencies. You can install them via pip:
   ```bash
   pip install fastapi>=0.139.0 fastapi-users[sqlalchemy]>=15.0.5 aiosqlite>=0.22.1 imagekitio>=5.7.0 python-dotenv>=1.2.2 streamlit>=1.59.1 uvicorn[standard]>=0.50.2
   ```
3. Create a `.env` file in the root of your project and configure your ImageKit credentials:
   ```env
   IMAGEKIT_PUBLIC_KEY=your_public_key
   IMAGEKIT_PRIVATE_KEY=your_private_key
   IMAGEKIT_URL=your_imagekit_url
   ```

## Running the Application

### 1. Start the FastAPI Backend
Ensure your virtual environment is activated and run the main entry point for the backend:
```bash
python main.py
```
*(This executes `uvicorn.run("app.app:app", host="0.0.0.0", port=8000, reload=True)` to start the backend API).*

### 2. Start the Streamlit Frontend
In a new terminal window, start the Streamlit application:
```bash
streamlit run frontend.py
```
*(Replace `frontend.py` with the actual name of your Streamlit script).*
