# IMDb Data Extraction Project
## Introduction
The IMDb Data Extraction Project aims to gather comprehensive information about the top 20 movies listed under each genre on IMDb, including movie details and the latest 10 user reviews for each movie. This data will be valuable for conducting a broad analysis of movie trends and reception across various genres.
## Project Components
### 1. Genre Identification
The script identifies and lists all movie genres available on IMDb dynamically. It adapts to any number of genres listed on the site.
### 2. Top 20 Movies Extraction
For each genre, the script extracts details of the top 20 movies, including movie title, year of release, director, cast, IMDb rating, and other pertinent information.
### 3. Reviews Extraction
For each of the top 20 movies, the script extracts the latest 10 user reviews, including review text, user rating, and date of the review.
### 4. Handling Dynamic Content
The script addresses challenges posed by dynamic content loading, such as JavaScript-rendered pages or pagination.
## Implementation Details
### Libraries Used
requests: Used for making HTTP requests to IMDb.
BeautifulSoup: Used for parsing HTML content.
json: Used for handling JSON data.
time: Used for introducing delays in the script.
random: Used for generating random delays.
### File Structure
main_script.py: The main script containing the IMDb data extraction logic.
top_20_movies.json: JSON file storing details of the top 20 movies for each genre.
movies_details.json: JSON file storing detailed information about each movie.
last_processed_rank.txt: Text file storing the rank of the last successfully processed movie.
## Usage Instructions
### Setup:
Install the required libraries using pip install requests beautifulsoup4.
### Run the Script:
Execute main_script.py to start the data extraction process.
### Output:
Extracted data is stored in top_20_movies.json and movies_details.json.
The script uses last_processed_rank.txt to resume from the last successfully processed rank.
## Known Issues
Handling potential network errors or connection issues.
## Future Enhancements
Implementing multi-threading for faster data extraction.
Adding error handling for various edge cases.
## Conclusion
The IMDb Data Extraction Project provides a foundation for gathering and analyzing movie-related data from IMDb. It can be extended and enhanced to cater to specific research or analytical requirements.

