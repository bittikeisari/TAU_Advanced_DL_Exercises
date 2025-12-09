# Setup Guidelines

All exercises will be implemented in Python and course assignments will be provided in **Jupyter Notebook** format. We will be using **PyTorch** as our primary deep learning library in Python.

To simplify setup and prevent issues related to package dependencies, we are providing a **Conda environment file**, which will be used for all assignments throughout this course. It is strongly recommended that you complete your implementations within the provided Conda environment to avoid any compatibility issues or version conflicts that may occur during grading.

Below is a step-by-step guideline to help you configure the setup required for the course assignments.

**Note**: Exercise**X** can be completed using a CPU, but it is recommended to use a GPU for faster computation for Exercise**X**. For those without access to a local GPU, Google Colab offers free GPU resources (see instructions below).

## 1. Setting up Conda Environment

Conda is an environment and package manager that allows you to create separate and isolated environments for different projects. By using a Conda environment, you can make sure that the packages in your local system is not broken by installing or updating packages. If you are not familiar with Conda, we encourage you to adopt to Conda environments for this course and beyond as it helps keep things organized and prevents dependency issues.

### Step 1: Install Conda

You can install Anaconda by following the instructions [here](https://docs.anaconda.com/anaconda/install/) for platform-specific installation steps. 

### Step 2: Create the conda environment


To run the exercises in this course, you need to create a Conda environment using the provided environment files. Use the appropriate file based on your operating system:

-   **macOS:** `mac_environment.yml`
-   **Windows:** `windows_environment.yml`

Then run the following code accordingly:

```bash
conda env create -n dl_course -f mac_environment.yml
```

(If you are on Windows, replace `mac_environment.yml` with
`windows_environment.yml`.)

This will create an environment with all the required dependecies used in this course. You should be able to see the created environment `dl_course` among your Conda environments by running:

```bash
conda env list
```

### Step 3: Activate the conda environment

After the environment is created, you need to activate it:

```bash
conda activate dl_course
```

## 2. Working with Jupyter Notebook

### Step 1: Launch Jupyter Notebook
Jupyter Notebook is installed in the `dl_course` environment. Once your Conda environment is activated, you can launch Jupyter Notebook by running:

```bash
jupyter-notebook
```

This will automatically display the Jupyter Notebook interface in a new tab in your default browser. If it does not automatically open, you can go to the URL provided in the terminal manually.

### Step 2: Running the Notebooks

In the Jupyter Notebook interface, navigate to the folder containing the assignment. The notebook files have the extension of `.ipynb` and they are designed to run Python code. The interface is organized into *cells*, that is used to break the code blocks in different chunks. You need to run the cells in consecutive order for the notebook to work properly. You can run each cell from either the toolbar or keyboard shortcut (default is `Shift + Enter`).

**Important notes**

**Note 1: Do not modify the provided code outside of the marked sections**
In the assignments, you are given a template code and expected to implement only the sections commented with `# YOUR CODE HERE`. **Do not** alter the rest of the code. You will also notice some cells are read-only. These cells are used to set default values and you **should not** overwrite them. Additionally, **do not** delete any cells from the original assignment file (even if you replicate them) as this might cause issues during grading. If you need extra space to try out different values or test your code, do so by inserting new cells either using the Insert option in menu bar or keyboard shortcuts (defaults are `ESC + A` to insert above and `ESC + B` to insert below). Before submitting, make sure that you remove any extra cells that were not in the original assignment file.

**Note 2: Passing the provided tests does not guarantee full marks** 
Each assignment will contain test cases for you to verify your implementation. As you progress through the notebook, you will get information on whether a test is passed. Keep in mind that additional test cases will be run after you submit your code: even if your implementation passes all the provided tests before the submission, this does not guarantee that you will receive full points.

## 3. Working with Google Colab (for GPU access)

For students who do not have access to a local GPU, [Google Colab](https://colab.research.google.com/notebooks/basic_features_overview.ipynb) offers free GPU resources. 

