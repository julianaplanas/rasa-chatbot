# Medical Appointment Scheduler

## Context
This virtual assistant is designed for use in a healthcare organization that provides medical services to patients. The assistant helps streamline the process of scheduling appointments, ensuring patients can easily book consultations with specialists.

## Overview
This project is a conversational bot designed to help users schedule medical appointments. The bot interacts with users to collect the patient's name, the desired appointment date and the doctor's specialty and then confirms the appointment.

## Features
- Collects the patient's name.
- Collects the desired date for the appointment.
- Collects the doctor's specialty.
- Confirms the scheduled appointment.

## Flows
### 1. Schedule Medical Appointment
**Description**: The assistant helps users schedule a medical appointment by collecting the patient's name, the desired appointment date and the doctor's specialty.
**Dialog Flow**:
1. The bot asks: "What is the patient's name?"
2. The user provides the name.
3. The bot asks: "What date would you like to schedule the appointment for?"
4. The user provides the date.
5. The bot asks: "What type of doctor do you need to see? (e.g., cardiologist, dermatologist)"
6. The user provides the specialty.
7. The bot responds: "Your appointment with a [Specialty] has been scheduled for [Date], [Name]."

## How to Use

### 1. Install Dependencies
Ensure you have Python 3.11 installed. Create a virtual environment and install the required dependencies:
```bash
python3.11 -m venv venv
source venv/bin/activate
pip install rasa-pro
```

### 2. Train the Bot
Train the bot using Rasa:
```bash
rasa train
```

### 3. Run the Bot
Start the Rasa server:
```bash
rasa inspect
```

## Project Structure
- **`config.yml`**: Configuration for the bot's pipeline and policies.
- **`domain.yml`**: Defines intents, slots, responses and actions.
- **`data/flows.yml`**: Contains the conversational flow for scheduling medical appointments.
- **`actions/actions.py`**: Custom actions for scheduling the appointment.

Enjoy using the Medical Appointment Scheduler!