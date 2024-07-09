## 🚩Analysis of Public Perception of Airbnb in Spain Tourist

✅Understanding Public Sentiment: Gauging how the public perceives women's participation helps stakeholders understand the level of support or opposition. This can influence policies, sponsorship, and media coverage.

✅Identifying Areas for Improvement: Sentiment analysis can highlight specific areas where women's participation is either praised or criticized, allowing organizations to address these issues effectively.

✅Promoting Equality: By continuously monitoring and analyzing public opinion, we can promote equality in sports, ensuring that women receive the recognition and opportunities they deserve.

✅Supporting Decision Making: Organizations, advertisers, and policy-makers can use these insights to make informed decisions that support and promote women's sports.

# 🚩Purpose of the Analysis

The purpose of this analysis is to understand how the Airbnb service in spanish tourism is perceived. Through sentiment analysis of posts and comments on Reddit, we aim to identify positive, negative, and neutral opinions on this topic. This information can be useful for political organizations, journalists, and analysts who wish to understand public perception and make informed decisions.

1. APIs Used

✅PRAW (Python Reddit API Wrapper): To access posts and comments on Reddit.
✅Transformers by Hugging Face: To use pre-trained sentiment analysis models.
✅NLTK (Natural Language Toolkit): For sentence tokenization.
✅Plotly: For data visualization.

2. Model Used (Pipelines)

We used the cardiffnlp/twitter-roberta-base-sentiment sentiment analysis model provided by Hugging Face. This model is optimized for analyzing sentiments in short texts, such as social media posts and comments.

💾Project Setup
APIs and Libraries Used
PRAW (Python Reddit API Wrapper): To access posts and comments on Reddit.
Transformers by Hugging Face: To use pre-trained sentiment analysis models.
NLTK (Natural Language Toolkit): For sentence tokenization.
Plotly: For data visualization.
Model Used (Pipelines)
We used the cardiffnlp/twitter-roberta-base-sentiment sentiment analysis model provided by Hugging Face. This model is optimized for analyzing sentiments in short texts, such as social media posts and comments.

💻Installation
Prerequisites
Python 3.8 or higher
pip (Python package installer)
Steps
Clone the repository:

git clone https://github.com/tu-usuario/nombre-del-repositorio.git
cd nombre-del-repositorio
Create and activate a virtual environment (optional but recommended):

python -m venv myenv
source myenv/bin/activate  # On Linux/Mac
myenv\Scripts\activate     # On Windows
Install the required packages:

pip install -r requirements.txt
Configure your Reddit API credentials: Create a file named config.ini in the root directory of the project with the following content:

[reddit]
client_id = YOUR_CLIENT_ID
client_secret = YOUR_CLIENT_SECRET
user_agent = YOUR_USER_AGENT
🚩Usage
Run the sentiment analysis script:

python app_roberta.py
Visualize the results: The script will output various visualizations using Plotly, including bar charts, scatter plots, pie charts, and box plots.

©️Explanation of the Code
Import Libraries and Configure Models
We import the necessary libraries, including PRAW for accessing Reddit, NLTK for text processing, Hugging Face's Transformers for sentiment analysis, and Plotly for data visualization. We also configure the sentiment analysis model.

Functions for Text Processing and Sentiment Analysis
split_text_into_chunks(text, tokenizer, max_length=512): Splits text into chunks that fit within the model's maximum token length.
analyze_text_chunks(text): Analyzes each chunk of text for sentiment.
aggregate_sentiments(sentiments): Aggregates the sentiment scores of the chunks into a single score.
Fetch Data from Reddit
fetch_reddit_posts_and_comments(): Fetches posts and comments from the euro2024 subreddit that mention "women".
Processing and Sentiment Analysis
We fetch the texts, process them to analyze sentiments, and aggregate the results.

Calculate Loss Rate and Display Results
We calculate the total number of texts processed, the number of errors, and the loss rate. The results are printed to the console.

Data Visualization
We use Plotly to create various visualizations to represent the sentiment analysis results.

Bar Chart: Shows the distribution of sentiments.
Scatter Plot: Displays sentiment scores for each text.
Pie Chart: Illustrates the proportion of each sentiment type.
Box Plot: Shows the distribution of sentiment scores within each sentiment category.

## 8. Conclusions

Through this analysis, we have gained significant insights into the public perception of Airbnb's service within the context of Spanish tourism during the summer of 2024, particularly concerning the phenomenon of tourism saturation and the touristification of residential neighborhoods.

🚩Distribution of Sentiments: According to the results, the majority of comments are neutral (44.2%), which could reflect a resigned acceptance of the service amidst growing concerns about tourism saturation. Negative comments account for 32.5%, suggesting significant criticism likely centered around the negative repercussions of tourism on the local community, such as neighborhood identity loss and rising prices. Positive comments make up 23.3%, indicating that although there are satisfied users, they are fewer in comparison to more critical or neutral views.

🚩Proportion of Sentiments: This chart highlights that the neutral and negative perceptions might be influenced by the view that Airbnb contributes to broader issues like touristification, which affects the quality of life of permanent residents and transforms neighborhoods into areas primarily oriented towards tourism.

🚩Sentiment Scores: The variability in scores could be indicative of the diverse experiences of users, fluctuating between the utility of the service and its negative impact on local communities.

🩹Implications for Airbnb:

✅Response to Tourism Saturation: It is crucial for Airbnb to implement strategies that mitigate the negative effects of mass tourism, such as supporting regulations that limit the number of properties available for short-term rentals in critical areas.

✅Promotion of Responsible Tourism: Encouraging a culture of responsible tourism among Airbnb users, highlighting the importance of respecting local communities and their traditions.

✅Community Integration Initiatives: Developing programs that better integrate tourists with local communities, supporting community-beneficial projects, and ensuring that a portion of the revenue generated by Airbnb contributes to local development.

This analysis provides a clear view of how Airbnb's service is perceived in relation to contemporary tourism challenges, offering a basis for future strategies that seek not only to improve the service's perception but also address the socioeconomic impacts on host communities.
