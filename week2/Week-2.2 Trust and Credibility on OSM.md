# Trust and Credibility in Online Social Media  
**Week 2.2 – Privacy and Security in Online Social Media (NPTEL Course)**  

This lecture (40 minutes) focuses on **trust and credibility analysis** in online social media.

---

## 🧩 The Core Problem: Rumors vs. Truth

- **Observation:** Rumors spread significantly faster than truth on social media.  
- **Case:** *Boston Marathon blast*  
  - Rumors peaked within **2 hours**, while truth took **~9 hours** to emerge.  
  - This time gap causes major challenges for **crisis management** and **public safety**.

---

## 🌪️ Real-World Case Studies

### **Hurricane Sandy (October 2012)**
- **Data Scale:** 1,782,526 tweets from ~1 million users  
- **Problem:** Circulation of multiple fake images (e.g., shark photos, manipulated disaster scenes)  
- **Ground Truth:** *The Guardian* verified fake/real images  
- **Key Insight:** ~600,000 tweets contained URLs → misinformation spreads via links  

### **Boston Marathon Blast (April 2013)**
- **Dataset:** 7.8 million tweets from 3.6 million users  
- **Fake Content Examples:**
  - False claim about an 8-year-old boy dying (50,000+ retweets)  
  - Scam tweets promising “$1 donation per retweet”  
- **Account Analysis:**  
  - 32,000 new accounts created  
  - 90% later suspended or deleted  
- **Network Pattern:** Fake content creators formed tightly connected, closed communities  

---

## 🔬 Research Methodology Framework

A systematic **five-step process** for social media analysis:

1. **Data Collection:** From Twitter/social platforms using APIs  
2. **Data Characterization:** Analyze volume, timeline, geographic distribution  
3. **Feature Extraction:** From posts and user profiles  
4. **Model Building:** Using machine learning algorithms  
5. **Evaluation:** With metrics like **Accuracy** and **NDCG (Normalized Discounted Cumulative Gain)**  

---

## 🧭 Who-When-Where-What-Why-How Analysis

| Dimension | Description |
|------------|-------------|
| **Who** | User profiles, follower networks, account age |
| **When** | Temporal patterns, posting timelines |
| **Where** | Geographic data (1% of tweets are geo-tagged) |
| **What** | Content analysis, sentiment, URLs |
| **Why/How** | Inferred from posting behavior and patterns |

---

## ⚙️ Feature Engineering: The Foundation

### **User (Profile-Based) Features**
- Number of followers and friends  
- Follower-to-following ratio *(celebrities have high ratios)*  
- Verification status *(verified = more credible)*  
- Account age *(older = more trustworthy)*  
- Number of times listed *(expert recognition)*  
- Profile completeness *(URL, bio, etc.)*

### **Tweet (Content-Based) Features**
- Tweet length and word count  
- Presence of question/exclamation marks  
- Emoticon usage (😊/😢)  
- URL presence and reputation *(WOT scores)*  
- Swear words and sentiment (positive/negative emotion)  
- YouTube video like/dislike ratios for linked videos  

---

## 🤖 Machine Learning Results

**Classification Techniques:**
- **Naive Bayes:** Probability-based  
- **Decision Trees:** Graph-based  

**Evaluation:** Five-fold cross-validation  

**Accuracy:** **97.65%** (when combining tweet + user features)  

**Findings:**
- Tweet features alone > user features alone  
- Combination of both → best performance  

---

## 🔝 Top 10 Most Influential Features

1. Number of characters in tweet  
2. Unique characters in tweet  
3. Number of words  
4. User has location in profile  
5. Number of retweets  
6. Age of tweet  
7. Tweet contains URL  
8. Tweet source (device used)  
9. User’s status count  
10. Followers-to-friends relationship  

---

## 🧑‍🏫 Human Annotation Process

**Two-Step Annotation:**
1. Check if the tweet is event-related  
2. Rate credibility:  
   - Definitely credible  
   - Seems credible  
   - Definitely not credible  
   - Can’t decide  

**Quality Control:**
- Each tweet annotated by ≥3 people  
- **Cronbach’s Alpha > 0.7** ensures inter-annotator agreement  

**Results:**
- 30% credible  
- 70% non-credible  
- 14% uncertain  

---

## 🌐 Network Analysis Insights

- **Diffusion Patterns:** Single-user vs. multi-user cascades  
- **Observation:** Content spreads fast even if original user isn’t influential  
- **Fake Content Networks:** Closed, dense communities (mutual follows/retweets)  

---

## 🧩 Practical Application: TweetCred Chrome Extension

**Purpose:** Real-time credibility scoring for tweets  

**Features:**
- Displays credibility score (1–7 scale)  
- Works on Twitter timelines, searches, and profiles  
- Uses 45 features (optimized subset for speed)  
- Allows user feedback (“I agree” / “This should be more credible”)  

**Implementation:**
- Real-time display integrated with Twitter interface  
- Feedback loop to improve model accuracy  

---

## 🧠 Key Takeaways for Practitioners

- **Speed Matters:** Misinformation spreads **4–5x faster** than truth  
- **Feature Combination:** Both content + profile features needed  
- **Temporal Patterns:** Tweet spikes align with real-world events  
- **Device Insight:**  
  - 76% of fake content → posted via **mobile**  
  - 64% of true content → via mobile  
- **Account Patterns:** Suspicious accounts often created right before/after major events  

---

## 🎯 Summary

This lecture provided **both theoretical foundations and practical tools** for identifying misinformation on social media.  
Applications include **crisis management**, **journalism**, and **digital literacy**.

---
