# 🌌 The Battle of Neighborhoods: Where You Should Live in Toronto Based on Your Zodiac Sign  
**Applied Data Science Capstone Project – IBM/Coursera**

🔗 _To view the interactive notebook with Folium Map: [Click here](#)_

## 1. 🌍 Introduction
At some point in our lives, most of us move to a new city—whether for education, career, or personal reasons. Toronto, the largest urban area in Canada and its financial hub, is a common destination for newcomers due to its diversity, safety, and high quality of life.

But with its variety of neighborhoods, choosing the right place to live can be overwhelming. What if your **zodiac sign** could guide you?

This project explores the whimsical idea of using **astrology and data science** together to suggest neighborhoods in Toronto that best align with personality traits associated with each zodiac sign.

## 2. 🔮 Business Problem
When choosing accommodation, people often prioritize tangible factors like rent, proximity to work or transit. But what about **personality fit**?

Some people thrive in vibrant, busy downtown areas, while others prefer quieter, laid-back neighborhoods. This project proposes a fun and exploratory solution:

> Can we recommend neighborhoods in Toronto that align with your zodiac sign's **personality traits**?

By analyzing venue types and neighborhood characteristics through data science, we aim to **cluster Toronto neighborhoods** and map them to zodiac archetypes.

## 3. 📊 Data Collection & Preprocessing

### 🏘️ Toronto Neighborhoods
- **Source:** [Wikipedia - List of Postal Codes of Canada: M](https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M)
- Extracted neighborhood and borough information using web scraping
- Used **Geocoder** to fetch latitude and longitude

### 📍 Venue Data
- **Source:** Foursquare API
- Fetched top venues for each neighborhood (e.g., parks, cafés, gyms, art galleries)
- One-hot encoding applied to venue categories to analyze frequency distribution

### ♒ Zodiac Sign Traits
- Zodiac personality characteristics (e.g., Aries: adventurous, Gemini: social)
- Collected from a publicly available source and saved as a CSV for integration

## 4. 🧪 Analyze Each Neighborhood
- Used frequency analysis to understand venue distribution in each neighborhood
- Created feature vectors representing the lifestyle offered by each neighborhood
- Explored which neighborhoods are artsy, outdoorsy, social, quiet, etc.

## 5. 🔗 Cluster Neighborhoods
- Applied **K-Means Clustering** to group neighborhoods with similar venue profiles
- Optimal number of clusters selected using elbow method
- Each cluster represents a **lifestyle archetype**

## 6. 🌠 Match Zodiac Traits to Clusters
- Interpreted each cluster based on dominant venues
- Matched clusters with zodiac traits to suggest where each sign may thrive

## 7. 💬 Discussion & Conclusion
This project takes a **light-hearted, pseudoscientific** approach to housing recommendation by blending **astrology and machine learning**. While not meant for serious real estate decisions, it demonstrates:

- How unsupervised learning can group urban spaces by behavior or lifestyle
- The potential of external personality models (like MBTI or Zodiac) in data-driven personalization

## 📌 Technologies Used
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `sklearn` (KMeans clustering)
- `folium` (interactive maps)
- `geopy`, `geocoder`, `requests`
- `BeautifulSoup` (for web scraping)

## 📜 License
This project is for educational and entertainment purposes. Zodiac personality traits are subjective and not scientifically validated.
