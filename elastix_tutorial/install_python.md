# Installing Python

## Overview
This how-to teaches how to install Python on your computer using `conda`, which is both a

- environment manager and a
- package manager.

### `conda` and `mamba`

There is one problem with conda: Its default package manager is very slow. Instead, using `conda` in combination with the package manager [`mamba`](https://mamba.readthedocs.io/en/latest/index.html) saves a lot of time when installing new packages. The version of `conda` which includes this package manager is called `mambaforge`.

**Prerequisites**
- You have a computer with linux, MacOS, or Windows installed

**Related reading**

- [mamba documentation](https://mamba.readthedocs.io/en/latest/index.html)

## Instructions

Select the installation instructions for your operating system and processor from the tabs below.

````{tab-set}
```{tab-item} Linux
1. In your web browser, navigate to this [download page](https://github.com/conda-forge/miniforge#mambaforge).
2. Scroll down to the "Mambaforge" header of the "Downloads" section. Click the link to download link for `Mambaforge-Linux-x86_64`.
3. Open your terminal application
4. Navigate to the folder you downloaded the installer to (usually this is in your Downloads folder). If the file was downloaded to your Downloads folder, you would enter:

    ```bash
    cd ~/Downloads
    ```   

5. Execute the installer with the command below. You can use your arrow keys to scroll up and down to read the license agreement and enter "yes" if you agree.

    ```bash
    bash Mambaforge-Linux-x86_64.sh
    ```
6. After installation, you will be asked if you would like to initialize your terminal with "conda init". Enter "yes" to initalize your terminal.
7. To verify your installation worked, close your Terminal window and open a new one. You should see `(base)` to the left of your prompt.

    ```{admonition} Don't see (base)?
    You can manually initialize conda by entering the command below and re-opening your terminal application.

    ```bash
    conda init
    
    ```

```

```{tab-item} Mac OS (Intel)
1. In your web browser, navigate to this [download page](https://github.com/conda-forge/miniforge#mambaforge).
2. Scroll down to the "Mambaforge" header of the "Downloads" section. Click the link to download link for `Mambaforge-MacOSX-x86_64`.
3. Open your Terminal (you can search for it in spotlight - `cmd` + `space`)
4. Navigate to the folder you downloaded the installer to (usually this is in your Downloads folder). If the file was downloaded to your Downloads folder, you would enter:

    ```bash
    cd ~/Downloads
    ```
    
5. Execute the installer with the command below.  You can use your arrow keys to scroll up and down to read the license agreement and enter "yes" if you agree.

    ```bash
    bash Mambaforge-MacOSX-x86_64.sh
    ```

6. After installation, you will be asked if you would like to initialize your terminal with "conda init". Enter "yes" to initalize your terminal.   
7. To verify your installation worked, close your Terminal window and open a new one. You should see `(base)` to the left of your prompt.
    
    ```{admonition} Don't see (base)?
    You can manually initialize conda by entering the command below and re-opening your terminal application.

    ```bash
    conda init
    ```

```

```{tab-item} Mac OS (M1/M2)
1. In your web browser, navigate to this [download page](https://github.com/conda-forge/miniforge#mambaforge).
2. Scroll down to the "Mambaforge" header of the "Downloads" section. Click the link to download link for `Mambaforge-MacOSX-arm64`.
3. Open your Terminal (you can search for it in spotlight - `cmd` + `space`)
4. Navigate to the folder you downloaded the installer to (usually this is in your Downloads folder). If the file was downloaded to your Downloads folder, you would enter:

    ```bash
    cd ~/Downloads
    ```
    
5. Execute the installer with the command below. You can use your arrow keys to scroll up and down to read it/agree to it.

    ```bash
    bash Mambaforge-MacOSX-arm64.sh
    ```
    
6. After installation, you will be asked if you would like to initialize your terminal with "conda init". Enter "yes" to initalize your terminal. 
7. To verify your installation worked, close your Terminal window and open a new one. You should see `(base)` to the left of your prompt.

    ```{admonition} Don't see (base)?
    You can manually initialize conda by entering the command below and re-opening your terminal application.

    ```bash
    conda init
    ```

```

```{tab-item} Windows
1. In your web browser, navigate to this [download page](https://github.com/conda-forge/miniforge#mambaforge).
2. Scroll down to the "Mambaforge" header of the "Downloads" section. Click the link to download link for `Mambaforge-Windows-x86_64`.
3. Find the file you downloaded (Mambaforge-Windows-x86_64.exe) and double click to execute it. Follow the instructions to complete the installation.
4. Once the installation has completed, you can verify it was correctly installed by searching for the "miniforge prompt" in your Start menu.
```
````