# How-to: Python in VS Code
_For MacOS_

### Step 1: Install Homebrew

Open a new terminal window and run the following code in the command line:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
See more about Homebrew and its install [here](https://docs.brew.sh/Installation).

### Step 2: Install Anaconda 

Using the same terminal, run the following code:
```
brew install --cask anaconda
```
[Anaconda](https://www.anaconda.com) will manage your Python install so you do not need to do this separately. 

### Step 3: Install VS Code

Download Visual Studio Code to your device [here](https://code.visualstudio.com/download).

Alternatively, you can do this on the same terminal using Homebrew:
```
brew install --cask visual-studio-code
```
### Step 4: Install Python extension for VS Code

Open the VS Code app and navigate to the **Extensions** tab on the left hand panel. Install the extension named _'Python'_ by Microsoft (usually the first in the list). 

Alternatively, when you create your first Python or Jupyter Notebook file, you will be prompted to do this. 

### Step 5: Create a workspace

Create a new folder on your device where you want to save your first project locally. 

In VS Code, navigate to the **Explorer** tab on the left hand panel and open your new folder within the app. This is your new **workspace**. 

### Step 6: Create Python environment 

Once your folder is opened within the **Explorer** panel, open the Command Pallette (⇧⌘P) and type _'Python: Create Environment'_, selecting this command. This will then give you the option to create a **Conda** environment, which will create this environment in your **workspace**. You will then be asked to select the appropriate version of Python for your environment. 

**NB**: The `.conda` file is hidden. Therefore, when you open the folder locally you will not see it, but it will appear in your **workspace** through **Explorer**.

### Step 7: Create file/notebook

Create a new file (**Python File** or **Jupyter Notebook**) within the **workspace** and save it locally. Select the '_.conda_' kernel. 

### Step 8: Run terminal in VS Code to install packages

Open a new terminal within VS Code. You will know it is correct if the name of your **workspace** appears in the command line, and it is prefixed with `.conda`. 

You can install packages here, such as [Splink](https://moj-analytical-services.github.io/splink/getting_started.html), by using the following command:

```
conda install -c conda-forge splink
```

Packages can also be installed using `pip` in the same environment. 

You should then be able to import this package directly in your Python file. 

**NB**: If you selected a **Jupyter Notebook** file, you will need to install [_ipykernel_](https://pypi.org/project/ipykernel/). You can do this in the VS Code terminal using the command `conda install ipykernel`. Alternatively, when you try and run your first code block you will be automatically prompted to complete this install. 

<br />

You should now have a working Python environment in VS Code. If you wish to create a new folder (or **workspace**) to start a different project, you will have to go back to **Step 6**. 