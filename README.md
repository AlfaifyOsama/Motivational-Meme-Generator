# Project Overview
This project sets up a flask web application that either randomly
generates memes (An image with text and a quote author) or lets the user 
type in text and the author.
# Running the program

 1. Run 'python main.py' from command line which gives the meme path as output.
 2. For flask mode run app.py from command line which runs flask on port 3000.
 3. Open a web browser and paste the url generated while running the app.py
 4. Initially it creates a random meme but for custom meme click create and provide the necessry inputs
 5. Then if you click create meme it will show generated meme.

# Roles & Responsibilities of submodules
The `QuoteEngine` submodule handels the ingestion and creation of quote objects.
The Ingestor class takes a file path and automatically chooses the fitting Ingestor
subclass to read the quotes and return a list of quote objects.

The `MemeEngine` loads the image, resizes if necessary, adds the quote and
saves the meme under the specified path.