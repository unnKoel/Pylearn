## Notes of python learning
take notes to record the knowledge and path of python learning.

#### Basic book link I'v read
[Free Python Tutorial For Beginners: Learn Python](https://python.land/python-tutorial), which is easy and frendly for newcomer to learn.

#### Development env builds in VS Code
reference as [Getting Started with Python in VS Code](https://code.visualstudio.com/docs/python/python-tutorial)

Summarize the steps as follows:
- First install python interpreter.
- Install python extension in VS Code and create virtual python env.
- At last create a python file to run and debug using both interpreter and python extension installed.

#### Formatting and linting
reference as [Linting Python in Visual Studio Code](https://code.visualstudio.com/docs/python/linting#_pylint)

Under current vitrual environment, Install corresponding Python packages like `autopep8` for foramtting, `pylint` for linting through following commands like 

```sh
pip3 install autopep8
pip3 install pylint
```
To customize linting option, create a `.pylintrc` option file in the workspace folder to specify options, The command to create that file likes below.

```sh
pylint --generate-rcfile > .pylintrc
```

#### Issues
- how to call Parent class methods within the overridden methods?

    There are two ways. one is Parent’s class methods can be called by using the Parent classname.method inside the overridden method. another is using super().
    
    refer to [Python: Call Parent class method](https://www.geeksforgeeks.org/python-call-parent-class-method/)

- The message `Activate.ps1 is not digitally signed. You cannot run this script on the current system.` is showed while activate virtual environment in Windows operating system.
    
    temporarily change the PowerShell execution policy to allow script to run by excuting following command.

    ```console
    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
    ```

#### Tools recommendation
- Jupyter notebooks
  
  Using this tool makes notes descriptive and including the runable python statements as examples. it's capable of recording your whole learning process and can be reused as other's reference that should really be called as self-document. It support to mix using markdown syntax and python statements to take notes.

  The Python extension of VS Code directly has this tool, Once you'v installed it, can directly use Jupyter notebooks, Refer to [Jupyter notebooks](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) 

#### Reading later
- [Developing in WSL](https://code.visualstudio.com/docs/remote/wsl)
- [Remote development in WSL](https://code.visualstudio.com/docs/remote/wsl-tutorial)
