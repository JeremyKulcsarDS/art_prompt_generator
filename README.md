# Artistic Picture Generation with ChatGPT and Mid-Journey

This repository contains code for generating artistic pictures by leveraging OpenAI's ChatGPT and Mid-Journey. The combination of these two models allows for the generation of prompts that inspire Mid-Journey to create unique and visually captivating artworks.

Please note that the Mid-Journey part of the process is manually done on a private Discord server. The outputs generated by Mid-Journey can be found in the "midjourney_outputs" folder of this repository.

## Installation

1. Clone the repository to your local machine using the following command:  
```git clone https://github.com/JeremyKulcsarDS/artistic-picture-generation.git```

2. Install the required dependencies by running:  
```pip install -r requirements.txt```

## Usage

DISCLAIMER: The usage of this notebook requires to have a properly configured ```.env``` file with an OpenAI key and base, as well as access to Mid-Journey on your platform of choice.

1. In the notebook, after defining the classes and functions, define the audience and give your features of choice:  
```audience = Audience(age='18-22', attributes=['energetic', 'undergraduate', 'aspiring computer scientist'])```

3. Use the ```brainstorm_ideas``` function to generate a prompt:  
```brainstorm_ideas(**audience.model_dump())```

4. Manually the content of the "detail" field and use it as a prompt for Mid-Journey. This will give the final output.

## To-do list

1. Make the notebook into a .py file accepting args from a console and later callable from a web UI

2. Build a pipeline to integrate Mid-Journey directly and skip the manual copy/paste part

## Contact
For any inquiries or feedback, please contact chankahei@xentropy.co or jeremy.kulcsar@diamondhill.io

Feel free to modify the sections and content as per your specific needs. Provide accurate installation instructions, usage examples, and relevant details about the project to help users understand and utilize the code effectively.
