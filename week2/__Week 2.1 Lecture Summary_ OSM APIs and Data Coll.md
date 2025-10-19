

# **Week 2.1 Lecture Summary: OSM APIs and Data Collection Tools**

## **Course Progress Recap**

Professor PK reminded students about **Assignment 1** (deadline: end of Week 2) and encouraged active forum participation by reading existing posts before asking questions.[^1][^7]

**Week 1 covered**: Types of social networks, massive data generation (400 hours YouTube videos uploaded per minute, 3.3M Facebook posts), the 5 V's of social media (Volume, Velocity, Veracity, Variety, Value), real-world impacts including compromised accounts and fake content, plus Linux and Python basics.[^7][^8]

## **Week 2.1 Core Concepts**

### **APIs (Application Programming Interface)**

APIs create a programmatic tunnel between your code and social media services for data collection. When you send a request (e.g., "give me PK's friends list"), the service responds with requested data. The course focuses on Facebook and Twitter APIs, though most platforms offer APIs.[^2][^1][^7]

**Critical limitation**: Rate limits prevent unlimited data collection - social media companies restrict how much data you can extract per timeframe.[^7]

### **Programming Language: Python**

Python is the preferred language for API requests due to extensive libraries supporting URL reading, data parsing, API interaction, and JSON object handling.[^7]

### **Data Formats**

**JSON (JavaScript Object Notation)**: Primary format for API responses. Example structure:

```json
{
  "id": "12345",
  "name": "Username"
}
```

APIs return data as JSON objects that can be visualized using JSON Viewer (jsonviewer.stack.hu) to understand field structure.[^7]

**XML (Extended Markup Language)**: Alternative format similar to JSON that some services use.[^7]

### **Database Storage**

**MySQL**: Traditional relational database storing data in rows and columns. Use simple SQL queries like `SELECT user_id, user_screen_name` to retrieve stored Facebook/Twitter data.[^7]

**MongoDB**: Modern NoSQL database increasingly popular for social media data storage.[^7]

### **Data Viewing Tools**

**phpMyAdmin**: Interface for viewing MySQL databases.[^7]

**RoboMongo**: Interface for viewing MongoDB databases and exploring field structures.[^7]

### **Facebook Graph API**

Facebook stores all content as a **graph structure**. Users, friends, pictures, videos, and status updates are **nodes**, while interactions like comments and likes are **edges**. Every node has a unique numeric ID. This graph-based architecture is why Facebook's API is called the "Graph API".[^7]

**Tutorial will cover**: Creating secret keys, authentication procedures, specific data types available for collection, and implementation details.[^7]

## **Data Collection Workflow**

1. **API** → Request data from social media platform
2. **Python** → Write programs to handle API requests
3. **JSON** → Receive and parse response data
4. **MySQL/MongoDB** → Store collected data
5. **phpMyAdmin/RoboMongo** → View and query stored data

This framework enables you to programmatically collect, store, and analyze social media data for security and privacy research.[^7]
<span style="display:none">[^10][^3][^4][^5][^6][^9]</span>

<div align="center">⁂</div>

[^1]: https://onlinecourses.nptel.ac.in/noc23_cs13/preview

[^2]: https://nptel.ac.in/courses/106106146

[^3]: https://onlinecourses.nptel.ac.in/noc24_cs04/announcements?force=true

[^4]: https://www.scribd.com/document/726302777/Privacy-and-Security-in-Online-Social-Media-Unit-14-Week-11-Summary

[^5]: https://www.careers360.com/university/indraprastha-institute-of-information-technology-delhi/privacy-and-security-in-online-social-media-certification-course

[^6]: https://www.youtube.com/watch?v=qXQHF8Mq6BY

[^7]: https://www.pbsiddhartha.ac.in/LMS/eContent/MOOCS_Privacy_Security_in_Online_Social_Media.pdf

[^8]: https://archive.nptel.ac.in/content/syllabus_pdf/106106146.pdf

[^9]: https://www.slideshare.net/slideshow/privacy-and-security-in-online-social-media-intro-to-course/64785869

[^10]: https://www.youtube.com/watch?v=KvWWRz0KHR8

