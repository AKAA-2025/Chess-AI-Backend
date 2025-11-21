# Chess AI Backend Project  

## Development setup guide
**Make sure to have python and pip installed!**  

```bash
python -m venv venv
```  

If you're using Windows, run:  
```bash
.venv\Scripts\activate
```  

If you're using macOS / Linux, run:  
```bash
source .venv/bin/activate
```  

Now, install all dependencies:  
```bash
pip install --no-cache-dir -r requirements.txt
```  

After that, you can now run the server with:  
```bash
python app.py
```  

If you install new dependencies, dont forget to run:  
```bash
pip freeze > requirements.txt
```  

## Production setup guide
**Make sure to have docker installed**  

Build the container:  
```bash
docker build -t backend .
```  

Now you can run it:  
```bash
docker run -p 5000:5000 backend
```  

Or if you want to run it in detach mode:  
```bash
docker run -d -p 5000:5000 backend
```  
