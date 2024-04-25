<!---

BSD License

Copyright (c) 2022, Kevin Yamauchi
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice, this
  list of conditions and the following disclaimer in the documentation and/or
  other materials provided with the distribution.

* Neither the name of the copyright holder nor the names of its
  contributors may be used to endorse or promote products derived from this
  software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
OF THE POSSIBILITY OF SUCH DAMAGE.

-->

# Setting up your python environment

## Installing python via mambaforge

In this tutorial, we will install python via mambaforge, a distribution of anaconda python. However, if you already have anaconda, miniconda, mambaforge, or miniforge installed, those will work as well and you can skip to the next section.

To install python via mambaforge, follow the instructions [here](install_python.md).


## Setting up your environment

```{admonition} Using conda instead of mamba?
The following assumes that you have installed python using Mambaforge as [described above](install_python.md). If you are using a pre-existing installation of python via anaconda, miniconda, or miniforge, consider installing `mamba` into your existing installation using the command `conda install -c conda-forge mamba`. Alternatively, you can simply replace the `mamba` commands below with `conda`.

```

1. Open your terminal.
	- **Windows**: Open the "miniforge prompt" from your start menu
	- **Mac OS**: Open Terminal (you can search for it in spotlight - cmd + space)
	- **Linux**: Open your terminal application


2. Navigate to the `elastix_tutorial/notebooks` subdirectory of the directory you downloaded.

	```bash
	cd <path to downloaded repository>/elastix_tutorial/notebooks
	```


3. The file `environment.yml` contains the dependencies needed to run the notebooks, and it specifies a `conda` environment named `elastix_tutorial`. Create this environment from the file by entering the following command.

	```bash
	mamba env create --file environment.yml
	```

4. Once the environment setup has finished, activate the environment. If you successfully activated the environment, you should now see `(elastix_tutorial)` to the left of your command prompt.

	```bash
	conda activate elastix_tutorial
	```

5. Test your napari installation. Enter the command below and an empty napari viewer should open. You can close the window after it opens. Please note that it takes a bit of extra time to launch napari the first time.
	
	```bash
	napari
	```


6. Test and run your notebook installation. We will be using notebook for interactive analysis. Enter the command below and it should launch jupyter notebook book in a web browser. Navigate to the notebooks from there to open and work on them.

	```bash
	jupyter notebook
	```