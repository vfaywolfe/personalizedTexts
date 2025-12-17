# personalizedTexts
📖 AI-Personalized Textbook Engine
This repository contains a framework for transforming raw educational content into structured textbooks, which are then dynamically personalized for individual learners using Generative AI.

🚀 Project Overview
The goal of this project is to move beyond "one-size-fits-all" education. By utilizing student profiles (JSON), we transform generic HTML chapters into tailored learning experiences that align with a student's interests, reading level, and prior knowledge.

🏗️ Repository Structure
/prompts: The "brains" of the operation.

textbook_generation.txt: Instructions for the LLM to convert raw files (PDF/PPT/DOCX) into clean, structured Markdown/HTML.

personalization.txt: The logic that takes a generic chapter and a student JSON profile to rewrite the content.

/configs: Global configuration files.

student_profile_schema.json: The standard data structure for learner attributes.

pre_survey.md: The assessment included in Chapter 1 of every textbook.

/textbooks: The content library.

Each textbook folder contains chapters.

Each chapter contains a /raw folder for source material and a /personalized folder for student-specific HTML builds.

🛠️ Personalization Workflow
Ingestion: Raw source files are placed in textbooks/[book_name]/chapter_[n]/raw/.

Generic Build: Use the textbook_generation.txt prompt to create the generic.html version.

Profiling: A student profile is created based on the student_profile_schema.json.

Personalization: The personalization.txt prompt processes the generic.html + profile.json to output a unique version in the student's subfolder.

🌐 Web Viewing
This repository is configured for GitHub Pages. All HTML files are viewable in-browser.

Generic Chapters: https://<username>.github.io/<repo-name>/textbooks/<book>/chapter_1/generic.html

Personalized Chapters: https://<username>.github.io/<repo-name>/textbooks/<book>/chapter_1/personalized/<student_id>/index.html

📚 Documentation
Detailed architectural diagrams, prompt engineering notes, and schema definitions can be found in the
