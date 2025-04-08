# Getting started - app frontend and backend creation

## Step 1: Understand the story of creating the fitness application

Refer to the `docs/octofit_story.md` file to understand the goals and requirements for the OctoFit Tracker application.

## Step 2: Create the initial directory structure

Run the following command to create the required directory structure for the OctoFit Tracker application:

```bash
mkdir -p octofit-tracker/{backend,frontend}
```

## Step 3: Setup the backend Python virtual environment

1. Create a Python virtual environment in the `octofit-tracker/backend` directory:
   ```bash
   python3 -m venv octofit-tracker/backend/venv
   ```

2. Activate the virtual environment:
   ```bash
   source octofit-tracker/backend/venv/bin/activate
   ```

3. Create a `requirements.txt` file in the `octofit-tracker/backend` directory with the following content:
   ```text
   Django==4.1
   djangorestframework==3.14.0
   django-allauth==0.51.0
   django-cors-headers==4.5.0
   dj-rest-auth
   djongo==1.3.6
   pymongo==3.12
   sqlparse==0.2.4
   stack-data==0.6.3
   sympy==1.12
   tenacity==9.0.0
   terminado==0.18.1
   threadpoolctl==3.5.0
   tinycss2==1.3.0
   tornado==6.4.1
   traitlets==5.14.3
   types-python-dateutil==2.9.0.20240906
   typing_extensions==4.9.0
   tzdata==2024.2
   uri-template==1.3.0
   urllib3==2.2.3
   wcwidth==0.2.13
   webcolors==24.8.0
   webencodings==0.5.1
   websocket-client==1.8.0
   ```

4. Install the required packages:
   ```bash
   pip install -r octofit-tracker/backend/requirements.txt
   ```

## Step 4: Install MongoDB

1. Update the package list and install MongoDB:
   ```bash
   sudo apt-get update && sudo apt-get install -y mongodb
   ```

2. Start the MongoDB service:
   ```bash
   sudo service mongodb start
   ```

3. Verify the MongoDB service is running:
   ```bash
   sudo service mongodb status
   ```

   Ensure the output indicates that the service is active and running.
