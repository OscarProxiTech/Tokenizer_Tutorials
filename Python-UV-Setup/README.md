# Python Setup

## Windows 10/11

### Python Download Page
[Python Download Page](https://www.python.org/downloads/)

Download the second most recent major version. Example, if the current version is `3.13.x` instead download `3.12.x`.

Open the downloaded python installer. Click **Add to PATH** then proceed with the installation. **Restart your computer** after it has finished. 

Open **Windows Powershell** and run the following command:

```powershell
python --version
```

### UV Download: 
Open **Windows Powershell** with **Run as Administrator** and run the following command:
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```
**Restart your computer** after it has finished. 

Open **Windows Powershell** again and run the following command. 
```powershell
uv --version
```

## MacOS


## Setting up a Python Project

### Guided Runthrough using the AI Agent
1. Create a new folder with your project name, e.g. `PDF-Tool`. 
2. Open the folder inside your IDE.
3. Inside the empty folder copy the following script into your AI Agent's chat box and allow it to guide through the setup and installation process of your python project.

```markdown
### Initial Project Setup
1. Run the following uv command in the project directory to initialize the project: `uv init .`
2. After initialization, install a simple package to verify the environment setup: `uv add requests` 
3. Once the environment is set up, run the main.py file: `uv run main.py`
4. If main.py fails to run, troubleshoot and print any errors found. Test solutions based on common Python and UV runtime issues.
5. If main.py runs successfully, inform the user the setup is complete and prompt them to fill out basic info in pyproject.toml.
```

### Manual Commands
1. Open your new project folder and insid e the terminal run `uv init .`.
2. When complete, create your virtual environment using `uv add requests`. 
3. Select the new envrionment prompt box. 
4. Test the environment is working using `uv run main.py`. 
