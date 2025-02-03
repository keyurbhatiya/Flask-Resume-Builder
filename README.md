# Flask Resume Builder

This is a Flask-based web application that allows users to create and customize their resumes using different design templates.

## Features
- Users can select a design template for their resume.
- A form collects user details, including personal information, skills, and social media links.
- Users can upload an image for their resume.
- The resume is dynamically generated based on the chosen template.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/keyurbhatiya/Flask-Resume-Builder.git
   ```
2. Navigate to the project directory:
   ```sh
   cd flask-resume-builder
   ```
3. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

## Usage

1. Run the application:
   ```sh
   python init.py
   ```
2. Open a web browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```

## Routes

- **`/`** : Home page
- **`/design`** : Select a resume design
- **`/form/<string:design>`** : Fill out a form with resume details
- **`/upload`** : Process form data and generate resume

## Folder Structure
```
flask-resume-builder/
│-- static/
│   ├── img/  # Stores uploaded images
├── assets/  # Contains design-related files
│   │   ├── design1/
│   │   │   ├── css/
│   │   │   ├── js/
│   │   │   ├── image/
│   │   │   ├── preview/
│   │   ├── design2/
│   |   |   ├── css/
│   │   │   ├── js/
│   │   │   ├── image/
│   │   │   ├── preview/
│   │   ├── design3/
│   |   |   ├── css/
│   │   │   ├── js/
│   │   │   ├── image/
│   │   │   ├── preview/
│   │   ├── design4/
|   |   |   ├── css/
│   │   │   ├── js/
│   │   │   ├── image/
│   │   │   ├── preview/
│-- templates/
│   ├── home.html
│   ├── design.html
│   ├── form.html
│   ├── template1.html  # Resume design 1
│   ├── template2.html  # Resume design 2
│   ├── template3.html  # Resume design 3
│   ├── template4.html  # Resume design 4
│-- init.py
│-- README.md
```

## Dependencies
- Flask
- uuid
- os
- schedule

Install dependencies using:
```sh
pip install flask schedule
```

## Notes
- Ensure the `static/img/` directory exists for image uploads.
- The app runs in debug mode for development. Disable debug mode in production.


- **Author:** Keyur Bhatiya  
- **GitHub:** [Keyur Bhatiya](https://github.com/keyurbhatiya)

Happy Coding! 🎯🔥
