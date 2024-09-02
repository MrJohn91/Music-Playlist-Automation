# Music-Playlist-Automation

## Summary
This project explores the viability of using machine learning to automate the creation of music playlists for Moosic, a startup currently relying on human experts for playlist curation. As Moosic looks to scale operations, this project addresses whether machine learning can effectively replicate or improve upon human curation.

## Business Questions to Answer
- **Are Spotify's audio features able to identify similar songs as defined by humanly detectable criteria?**
- **Is K-Means a good method to create playlists?**
  - What are the pros and cons?
- **What audio features should be used or dropped, and why?**
- **Is the prototype effective at creating cohesive playlists?**
- **What kind of data might help us create better playlists?**
- **What are the next steps if we continue with this project?**

Through clustering songs based on audio features provided by Spotify, and automatically generating playlists, this project provides insights into the effectiveness of machine learning for this task and suggests possible next steps for Moosic's adoption of these technologies.

## Languages and Libraries Used
- **Python**
  - Libraries:
    - `pandas` for data manipulation
    - `numpy` for numerical computations
    - `scikit-learn` for machine learning models and PCA
    - `matplotlib` and `seaborn` for data visualization
    - `plotly` for interactive visualizations
    - `spotipy` for interacting with the Spotify API

## Key Learnings
Throughout this project, I gained skills in clustering techniques, specifically K-Means clustering, and Principal Component Analysis (PCA) for dimensionality reduction. I also learned how to evaluate clustering performance using methods like silhouette analysis and elbow method. Additionally, I developed proficiency in automating playlist creation using the Spotify API and improved my ability to communicate technical insights to non-technical audiences, a critical skill for data scientists.

## Challenges Overcame
One of the significant challenges in this project was determining the optimal number of clusters for the K-Means algorithm. Initially, the choice of clusters was somewhat misaligned, leading to less meaningful groupings. I addressed this by using the elbow method and silhouette analysis, which helped determine the optimal number of clusters by measuring how similar each song is to its own cluster compared to other clusters. This improved the quality of the generated playlists.

Another challenge was ensuring that the clustering algorithm could group songs in a way that aligns with human expectations for playlist cohesion. While K-Means worked well in many cases, it became clear that the subjective nature of music preferences means that no algorithm is perfect. Balancing the algorithm's output with human intuition was a key takeaway.

I also faced challenges with integrating the project with the Spotify API, specifically in terms of managing authentication, handling rate limits, and dealing with occasional API errors. For instance, when attempting to push multiple playlists to Spotify, errors related to token expiration and API limitations occurred. I overcame these challenges by implementing proper error handling and by clearly communication.

## Additional Reflections
This project highlighted the potential of machine learning to scale tasks like playlist creation, which traditionally rely heavily on human expertise. However, it also emphasized the limitations of purely algorithmic approaches in areas that require  judgment, such as music curation. Moving forward, a hybrid approach that combines algorithmic efficiency with human oversight might be the most effective strategy.

In terms of stakeholder communication, I ensured that technical details were translated into non technical  terms, focusing on how the project could scale playlist creation, while also outlining the limitations and suggesting a balanced approach that leverages both technology and human expertise.
