import requests

# Raw GitHub URL of your notebook
url = "https://raw.githubusercontent.com/samvincy7/pyin/main/AI_and_Automation_Lab.ipynb"

# Download and save the notebook file
response = requests.get(url)
with open("pyin_downloaded.ipynb", "wb") as f:
    f.write(response.content)

print("Notebook downloaded as pyin_downloaded.ipynb")
