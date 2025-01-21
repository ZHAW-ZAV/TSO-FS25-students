# TSO-FS25
Traffic System Operations, spring semester 2025

<a target="_blank" href="https://colab.research.google.com/github/ZHAW-ZAV/TSO-FS25">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## How to work
You have two options to work in this course: with a local installation of the conda/mamba environment or with Google Colab.

### Google Colab
Google Colab is a free cloud service that allows you to run Python code in a Jupyter notebook. It is a great way to work on the exercises in this course without having to install anything on your computer. The only thing you need is a Google account, which you can create when you first access Colab. However, it is not quite as convenient as working locally.

1. Either
  - Click on the `Open in Colab` badge at the top of this README.md file, or
  - Go to [Google Colab](https://colab.research.google.com/), click on `File` -> `Open notebook` -> `GitHub` and paste the URL of this repository.
2. Follow the instructions in the notebook.

If you have specific packages that you need to install, you can do so by running the following command in the notebook:
```python
!pip install package_name
```

However, it can take quite some time to install packages in Google Colab and needs to be repeated every time you restart the runtime. Additionally, the `traffic` package returns an error if installed with the command above.

Some notebooks have a code cell at the beginning that installs the necessary packages. You can run this cell by clicking on the play button in the cell or by pressing `Shift + Enter`.


### Local installation
It is also possible to work locally in this course. It is arguably more convenient to work locally, but you'll have to install an IDE like Visual Studio Code and mamba/miniforge.

1. In a command line, navigate to the folder where you want to keep this repository and clone it.
   ```bash
    cd path/to/your/folder
    git clone https://github.zhaw.ch/TraffSysOps/FS25.git
    ```
2. Install Miniforge by following the instructions [here](https://github.com/conda-forge/miniforge).
3. Create the environment by running the following command in the terminal:
   ```bash
   mamba env create -f environment.yml
   ```

You can activate the environment with the following command to use it in your terminal:
```bash
mamba activate tso-fs25
```
You can also use your favorite IDE to work with the environment. We recommend using [Visual Studio Code](https://code.visualstudio.com/) with the `Python` and `Jupyter` extensions. There is plenty of documentation on how to set up your environment with these tools and on the internet.

If you want to update your local copy of this repository, you can do so by running the following command in the terminal:
```bash
cd path/to/your/folder/FS25
git pull
```

If you want to update your environment, you can do so by running the following command in the terminal:
```bash
mamba env update -f environment.yml
```
