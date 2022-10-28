# Local Development Environment Setup

1. Navigate to the desired location of the repository via terminal.
    ```
    cd <path/to/dir>
    ```
2. Clone the `registry-database` repository from Github.
    ```
    git clone https://github.com/AHA-GitHub/registry-database.git
    ```
3. If not already installed, install `python3`.
    ```
    brew install python3
    ```
4. Create a new virtual environment using any environemnt management tool, preferably `conda`.
    ```
    conda create –n <name_of_env> python=3.9 
    ```
5. Activate the virtual environment.
    ```
    conda activate <name_of_env>
    ```
6. Install all packages in the `requirements.txt` file in your virtual environment using `pip`.
    ```
    pip install -r requirements.txt 
    ```
