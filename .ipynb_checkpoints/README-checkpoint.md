
# 🛍️ Customer Segmentation Using Unsupervised Learning

## 📌 Project Overview & Task Objective

The objective of this project is to segment customers into distinct groups based on their purchasing behavior using **unsupervised machine learning** techniques. By identifying meaningful customer segments, businesses can tailor marketing strategies, personalize services, and optimize customer satisfaction.

This project uses the **Mall Customers Dataset**, which contains demographic attributes such as `Age`, `Annual Income`, and `Spending Score` for mall customers. The goal is to discover natural customer groupings without any predefined labels.

---

## 📂 Dataset Information

The dataset includes the following key features:

- **CustomerID**: Unique ID for each customer  
- **Gender**: Male/Female  
- **Age**: Age of the customer  
- **Annual Income (k$)**: Income in thousands of dollars  
- **Spending Score (1–100)**: Score assigned by the mall based on customer spending patterns  

---

## 🚀 Approach

The project followed these key steps:

- **Data Exploration**: Visualized age, income, and spending patterns to understand customer distribution.  
- **Preprocessing**: Selected relevant features and scaled data using `StandardScaler` to prepare for clustering.  
- **Clustering**: Applied the KMeans algorithm. Used the Elbow Method to identify **5 optimal clusters**.  
- **Visualization**: Plotted 2D and 3D scatter plots to interpret the distinct customer groups visually.  

---

## 📉 Visualizations
 #### Age Distribution

 **Insights:**
- Majority of mall customers are aged 20 to 40.

- This shows that young and mid-age are possibly active shoppers.

 #### Gender Distribution

 **Insights:**
- Slight skew towards female customers.

- Marketing strategies could be tailored with a female-oriented focus.

 #### Income vs Spending Score by Gender

 **Insights:**
- People with the same income spend very differently.

- Some low earners spend a lot, and some high earners spend very little.

- This tells us that spending habits don't depend only on income, so grouping customers makes sense.

#### Optimal Cluster Selection (Elbow Method)

**Insights:**
- As the number of clusters increases, inertia (within-cluster variance) decreases.

- A sharp drop in inertia is observed up to k = 5.

- After k = 5, the rate of decrease slows, forming an "elbow" shape in the curve.

- This suggests that 5 clusters provide a good trade-off between performance and simplicity.

- Choosing more than 5 clusters leads to minimal gain in compactness while increasing complexity.

**Optimal number of clusters selected: k = 5**

## 📊 Results and Findings

### 🧠 Key Insights:

| Cluster       | Profile                                                                                      | Suggested Strategy                                                                              |
| ------------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| **Cluster 0** | 🧍 Age: \~33, High income (\~86k), **Very high spender** (82), Slightly more **females**     |  Show them new arrivals, premium brands, loyalty rewards, and early access to sales. |
| **Cluster 1** | 👩 Age: \~36, High income (\~89k), **Very low spender** (18), Slightly more **females**      |  Offer exclusive memberships, long-term value, and high-quality items. Focus on smart spending.     |
| **Cluster 2** | 👵 Age: \~50, Medium income (\~49k), Low spender (40), **All female**                        |  Promote useful, practical products with clear benefits. Use email or SMS offers.  |
| **Cluster 3** | 👧 Age: \~25 (youngest), Low income (\~40k), **High spender** (61), More **females**         |  Use trendy products, influencers, flash sales, and social media ads to grab attention.  |
| **Cluster 4** | 👨 Age: \~56 (oldest), Medium income (\~54k), Low spender (36), **All male**                 |  Focus on discounts, bundle offers, and simple loyalty programs. Keep it clear and value-based.  |


## 🧰 Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 💻 Usage

```bash
# Clone the repository
git clone https://github.com/your-username/customer-segmentation-unsupervised.git

# Navigate into the directory
cd customer-segmentation-unsupervised

# Open the notebook
jupyter notebook "Customer Segmentation using Unsupervised Learning.ipynb"
```

---

## 🤝 Contributing

Feel free to fork the repository, raise issues, or suggest improvements through pull requests.

---

## 📬 Contact

For questions or suggestions:  
- GitHub: `YourUsername`  
- Email: `youremail@example.com`  
