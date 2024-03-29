# Spelling Error Detection and Correction System 

This study aims to develop a Guragee spell checker that takes into account the complex morphology of the Gurage language.
Previous attempts using approaches like metaphone and edit distance algorithms, designed for simpler languages like English, 
did not yield satisfactory results for Gurage. Similarly, existing morphological analyzers were not suitable for computational morphology in Gurage. 
Therefore, this study explores the possibility of using a morphology-based approach to design and develop a Guragee typing error detection and correction system specifically targeting non-word errors.

 The code I provided leverages Flask to create a web application with route handling, form processing, and HTML template rendering using Jinja.
- *The code is a Flask application written in Python(app.y).*
- *It utilizes a SQL database(spellcheckersql.py).*
- *The application includes route handlers to handle different URL endpoints and execute corresponding functions(@app.route('/spellcheck', methods=['POST'])in app.py.*
- *Form handling is implemented to process user input from HTML forms.*
- *The Jinja template engine is used to render dynamic HTML templates by filling in data placeholders with Python code.*

![image](https://github.com/aronsinkie/NIDS/assets/74707268/1365abb1-e975-4979-9434-ec23c2bef5bb)


https://github.com/aronsinkie/NIDS/assets/74707268/978393a1-abca-4b71-873b-2c1fc88c8ecd




 ## General Architecture of the System
The spell checker works by accepting a block of text and splitting it into individual words. It analyzes each word for spelling errors and determines if it is valid or invalid. For incorrect words, the spell checker provides suggestions for alternative words based on their similarity in spelling, calculated using a distance algorithm. The suggestions are ranked based on the calculated distance, with closer words being given higher priority.
<p align="center">
  <img src="https://github.com/aronsinkie/NIDS/assets/74707268/567f3461-7aa6-4be9-9f8c-e0bd5f5e458b" width="400">
</p>

## Detailed Architecture of The System

The system makes use of a stored database called the dictionary, which comprises ten tables in the background. These tables encompass various components such as Morphological rules, Dictionary lookup, and the Amharic characters database. In addition, the system incorporates the dictionary searcher Ratcliff-Obershelp and the Distance Calculator component. These components are essential parts of the Rule Filter, Stem Extractor, and Suggestion Ranker components within the system.
<p align="center">
  <img src="https://github.com/aronsinkie/NIDS/assets/74707268/3ebd9e6c-f5c5-481a-add2-8cf741b72aec" width="400">
</p>

<div></div>



