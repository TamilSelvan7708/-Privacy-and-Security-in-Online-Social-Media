Perfect Summary: Trust and Credibility in Online Social Media (40-min
Lecture) Lecture Context This is Week 2.2 of the NPTEL “Privacy and
Security in Online Social Media” course, focusing specifically on trust
and credibility analysis.​

The Core Problem: Rumors vs. Truth The lecture opens with a critical
finding from the Boston Marathon blast analysis: rumors spread
significantly faster than truth on social media. Data showed rumors
peaked within 2 hours, while legitimate information took approximately 9
hours to emerge. This time gap creates massive challenges for crisis
management and public safety.​

Real-World Case Studies Hurricane Sandy (October 2012) Data Scale:
1,782,526 tweets collected from ~1 million unique users​

Problem: Multiple fake images circulated, including fabricated shark
photos and manipulated disaster scenes​

Ground Truth: The Guardian newspaper provided verified fake/real image
annotations​

Key Insight: Approximately 600,000 tweets contained URLs, showing how
misinformation spreads through linked content​

Boston Marathon Blast (April 2013) Massive Dataset: 7.8 million tweets
from 3.6 million users​

Notable Fake Content:

False claim about 8-year-old boy dying (50,000+ retweets)​

Scam tweets promising $1 donations per retweet​

Account Analysis: 32,000 new accounts created during the event; 90% were
later suspended or deleted​

Network Pattern: Fake content creators formed tightly connected, closed
communities​

Research Methodology Framework The lecture presents a systematic
five-step approach applicable to any social media analysis:​

Data Collection from Twitter/social platforms using APIs

Data Characterization (understanding volume, timeline, geographic
distribution)

Feature Extraction from posts and user profiles

Model Building using machine learning techniques

Evaluation using metrics like accuracy and NDCG (Normalized Discounted
Cumulative Gain)​

Who-When-Where-What-Why-How Analysis The lecture emphasizes analyzing
social media events through six critical dimensions:​

Who: User profiles, follower networks, account age

When: Temporal patterns, posting timelines

Where: Geographic data from geo-tagged tweets (1% of tweets have
location data)​

What: Content analysis, sentiment, URLs

Why/How: Harder to determine but inferable from patterns

Feature Engineering: The Foundation User Features (Profile-Based) Number
of followers and friends

Follower-to-following ratio (critical indicator: celebrities have high
ratios)​

Verification status (verified accounts are more credible)​

Account age (older accounts more trustworthy)​

Number of times listed (indicates expert recognition)​

Profile completeness (has URL, bio, etc.)​

Tweet Features (Content-Based) Tweet length and word count

Presence of question/exclamation marks

Emoticon usage (happy/sad)

URL presence and reputation (WOT scores)​

Swear words and sentiment (positive/negative emotion words)​

YouTube video like/dislike ratios for linked videos​

Machine Learning Results Classification Performance Using Five-fold
cross-validation with two algorithms:​

Naive Bayes: Based on probability theory

Decision Trees: Graph-based classification

Accuracy Achievement: 97.65% when combining tweet + user features​

Key Finding: Tweet features alone performed better than user features
alone, but the combination yielded the best results.​

Top 10 Most Influential Features The lecture identifies the most
powerful predictors of credibility:​

Number of characters in tweet

Unique characters in tweet

Number of words

User has location in profile

Number of retweets

Age of tweet

Tweet contains URL

Tweet source (posting device)

User’s status count

Followers-friends relationship

Human Annotation Process A rigorous two-step annotation methodology was
implemented:​

Step 1: Annotators decide if tweet contains event-related information

Step 2: If yes, rate credibility as “definitely credible,” “seems
credible,” “definitely not credible,” or “can’t decide”

Quality Control: Each tweet annotated by at least 3 people; Cronbach’s
Alpha (inter-annotator agreement) should be >0.7 for confident results.​

Results from annotation: 30% tweets had credible information, 70%
non-credible, 14% uncertain.​

Network Analysis Insights Visual network graphs revealed critical
patterns:​

Single-user diffusion vs. multi-user cascades

Content can spread rapidly even when original poster is not influential

Fake content networks show closed community structure (accounts follow
and retweet each other)​

Practical Application: TweetCred Chrome Extension A real-time
credibility assessment tool was developed and demonstrated:​

Features Provides credibility scores on a 1-7 scale for every tweet in
timelines, searches, and profiles​

Uses 45 features for real-time analysis (subset of research features for
speed)​

Feedback loop: Users can agree/disagree with scores to improve the model​

Implementation Works across Twitter interface showing immediate
credibility ratings, with options for users to provide feedback like “I
agree” or “No, this should be more credible”.​

Key Takeaways for Practitioners Speed Matters: Misinformation spreads
4-5x faster than truth during crisis events​

Feature Combination: Both content and profile features necessary for
accurate prediction​

Temporal Patterns: Tweet spikes on social media directly correlate with
real-world events​

Device Analysis: 76% of fake content posted via mobile vs. 64% true
content​

Account Patterns: Suspicious accounts often created immediately
before/after major events​

This lecture provides both theoretical foundations and practical tools
for identifying misinformation on social media platforms, with direct
applications in crisis management, journalism, and digital literacy.
