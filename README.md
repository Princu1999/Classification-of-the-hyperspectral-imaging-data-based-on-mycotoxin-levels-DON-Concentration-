# ImagoAI Classification Project

This project contains a classification implementation using Python. The main code is provided in the Jupyter Notebook `Princu_Singh_ImagoAI.ipynb`, which demonstrates data preprocessing, model training, and evaluation for a classification task.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Dependencies](#dependencies)
  - [Using a `requirements.txt` File](#using-a-requirementstxt-file)
  - [Installing Dependencies Manually](#installing-dependencies-manually)
- [Running the Classification Code](#running-the-classification-code)
- [Running the Streamlit App from Colab](#running-the-streamlit-app-from-colab)
- [Project Structure](#project-structure)
- [Additional Notes](#additional-notes)
- [License](#license)

## Prerequisites

- **Python 3.x**  
- **pip** (Python package installer)  
- **npm** (for installing Node packages)

## Dependencies

This project requires several Python libraries and additional tools. You can install them using one of the following methods.

### Using a `requirements.txt` File

If a `requirements.txt` file is provided in the repository, install all dependencies by running:

```bash
pip install -r requirements.txt
```

### Installing Dependencies Manually

To manually install dependencies without the `requirements.txt` file, use the following commands:

```bash
pip install numpy pandas matplotlib scikit-learn jupyter pytorch-tabnet optuna streamlit
```

### Additional Tools
Install Localtunnel using npm:

```bash
npm install -g localtunnel
```

## Running the Classification Code

The main classification code is contained within the Jupyter Notebook `Princu_Singh_ImagoAI.ipynb`. Follow these steps to run the code:

### Clone the Repository

Open your terminal and run:

```bash
git clone <repository_url>
cd <repository_directory>
```

### Launch Jupyter Notebook

Start Jupyter Notebook by running:

```bash
jupyter notebook
```

### Open and Run the Notebook

In the Jupyter Notebook interface, open the `Princu_Singh_ImagoAI.ipynb` file and execute the cells sequentially to run the classification workflow.

## Running the Streamlit App from Colab

If you wish to run a Streamlit app from within Google Colab, follow these steps:

### Install Streamlit (if not already installed)

Ensure Streamlit is installed by running:

```bash
pip install streamlit
```

### Generate an SSH Key in Colab

Run the following command in a Colab cell to generate an SSH key:

```bash
!ssh-keygen -t rsa -b 2048 -f /root/.ssh/id_rsa -q -N ""
```

### Connect Using Your Generated Key

Connect to localhost via SSH by running:

```bash
!ssh -i /root/.ssh/id_rsa -o StrictHostKeyChecking=no -R 80:localhost:8501 ssh.localhost.run
```

### Accessing the Streamlit App

If the command runs without error, it will display a public URL where your Streamlit app is accessible. If issues occur, please refer to the localhost.run FAQ for additional troubleshooting.

## Project Structure
```
├── dataset
│   └── <dataset_files>
├── notebooks
│   └── Princu_Singh_ImagoAI.ipynb
├── requirements.txt
└── README.md
```

## Additional Notes

- Ensure that your dataset files are placed in the `data/` folder before running the Jupyter Notebook.
- Trained models will be saved in the `models/` folder.
- For best results, ensure that all dependencies are correctly installed before proceeding.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

