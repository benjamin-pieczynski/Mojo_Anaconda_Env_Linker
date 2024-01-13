# Mojo_Anaconda_Env_Linker
Useful bash scripts to link the Mojo Python library to your anaconda environment on 'conda activate env' and deactivate it for 'conda deactivate'.

### Included Scripts

`init_mojoconda.sh`

When a conda environment is active, run this script to create an export-mojo.sh script that executes everytime the 'conda activate' command is invoked. The script also creates 'unset-mojo.sh' which unsets the MOJO_PYTHON_LIBRARY on 'conda deactivate'.

`mojo_env.sh`

Displays the current active MOJO_PYTHON_LIBRARY.

### Instructions

1.) Download the repository.

2.) Move the files to the desired directory and give them executabke premissions `chmod +x init_mojoconda.sh`

3.) Include an alias for each script in a .bash .bashrc .bash_aliases or .zshrc. ***Optional Step

4.) `source ~/.your_bash_file`

5.) Activate the conda environment you want to create a MOJO_PYTHON_LIBRARY link for. `conda activate your_env`

6.) run `init_mojoconda.sh` to create the mojo python link.

7.) `conda deactivate`

8.) `conda activate your_env`

9.) run `mojo_env.sh` to display the linked library path.
