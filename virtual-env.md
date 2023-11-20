# Anaconda Virtual Environment Cheat Sheet

## **1. Install Anaconda**

## **2. Open Anaconda Prompt**
- **Windows**: Search for "Anaconda Prompt" in your start menu.
- **macOS/Linux**: Open your terminal.

## **3. Creating a New Environment**
- `conda create -n myenv python=3.8`
  - Replace `3.8` with your preferred Python version.

## **4. Activating the Environment**
- `conda activate myenv`

## **5. Deactivating the Environment**
- `conda deactivate`

## **6. Installing Packages**
- With environment activated: `conda install numpy`
  - Replace `numpy` with the package you want to install.

## **7. Listing Environments**
- Run: `conda env list`
- Your current environment is marked with an asterisk (*).

## **8. Removing an Environment**
- Run: `conda remove --name myenv --all`
  - Replace `myenv` with the name of the environment you want to remove.

# Advanced

## **9. Exporting Environment File**
- Run: `conda env export > environment.yml`
- This creates an `environment.yml` file with your environment's package list.

## **10. Creating Environment from an Environment File**
- Run: `conda env create -f environment.yml`

## **11. Updating an Environment from a YAML File**
- Run: `conda env update --name myenv --file environment.yml`
  - Replace `myenv` with your environment's name.

## **12. List Packages in an Environment**
- Run: `conda list`

## Tips
- Ensure Anaconda is updated: `conda update conda`
- Check for specific package versions before installing: `conda search package_name`
- Use Anaconda Navigator (GUI) for a more visual approach.
