1. Train_files has the data


2. chatbot2 is the setup env. 

   -C:\Users\path\path\chatbot2\Scripts\activate.bat


3. pip install -r .\req.txt to install the dependencies


4. fix for llama_index and faiss-cpu ssl-encryption issue
   
   -pip install llama_index --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org

   -pip install faiss-cpu --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org

