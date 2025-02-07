#  **INDIAN GENERAL ELECTIONS RESULT 2024**

## 📌 **Overview**

This project contains SQL scripts and queries to analyze the results of the Indian General Elections 2024. The dataset includes details about constituencies, candidates, parties, and voting breakdowns, allowing comprehensive insights into election outcomes at the state and national levels.

---

## 📂 **Database Schema**

### 🗳️ **Tables and Their Purpose**

1. **`constituencywise_details`**

   - Stores candidate-wise vote details per constituency.
   - Fields: `S_N`, `Candidate`, `Party`, `EVM_Votes`, `Postal_Votes`, `Total_Votes`, `Percentage_of_Votes`, `Constituency_ID`.

2. **`constituencywise_results`**

   - Stores the winning candidate, total votes, and margin per constituency.
   - Fields: `S_No`, `Parliament_Constituency`, `Constituency_Name`, `Winning_Candidate`, `Total_Votes`, `Margin`, `Constituency_ID`, `Party_ID`.

3. **`partywise_results`**

   - Stores the number of seats won by each party.
   - Fields: `Party`, `Won`, `Party_ID`, `party_alliance`.

4. **`statewise_results`**

   - Stores state-wise election details, including leading and trailing candidates.
   - Fields: `Constituency`, `Const_No`, `Parliament_Constituency`, `Leading_Candidate`, `Trailing_Candidate`, `Margin`, `Status`, `State_ID`, `State`.

5. **`states`**

   - Stores state-level mapping.
   - Fields: `State_ID`, `State`.

---

## 🔍 **Key Queries and Insights**

### ✅ **Total Seats in the Election**

- Retrieves the total number of seats available for elections across all constituencies.

### 🏛️ **Seats Available Per State**

- Provides the number of seats contested in each state.

### 🏆 **Seats Won by Major Alliances (NDA & I.N.D.I.A)**

- Computes the total seats won by **NDA**, **I.N.D.I.A**, and **OTHER** alliances.

### 📊 **Seats Breakdown by Party and State**

- Displays party-wise seat counts for each state.

### 🔥 **Winning Candidates by State and Constituency**

- Lists the **winner, party name, alliance, total votes, and margin** for a specific state and constituency.

### ✉️ **EVM vs. Postal Vote Distribution**

- Shows the vote share of **EVM** and **postal ballots** for each candidate in a selected constituency.

### 🏅 **Top 10 Candidates with Highest EVM Votes**

- Identifies the **candidates who secured the highest number of EVM votes** across all constituencies.

### ⚔️ **Winning vs. Runner-up Candidates in Each State**

- Lists the **winner and the runner-up** in each constituency of a specified state.

### 📌 **Maharashtra Elections Breakdown**

- Provides a **detailed analysis** of Maharashtra elections, including:
  - **Total Seats**
  - **Total Candidates**
  - **Total Parties**
  - **Total Votes Cast (EVM + Postal)**
  - **Breakdown of EVM & Postal Votes**

---

## 🛠 **Modifications and Enhancements**

### ➕ **Adding Party Alliances Column**

- A new column `party_alliance` was added to `partywise_results` to categorize parties into:
  - 🟡 **NDA**
  - 🔵 **I.N.D.I.A**
  - ⚪ **OTHER**

### 🔄 **Updating Party Alliances**

- SQL `UPDATE` statements classify parties into their respective alliances.

### 🏆 **Alliance-Wise Winning Analysis**

- Queries calculate which **alliance won the most seats** across India.

---

## 📈 **Expected Outcomes**

✔️ Understanding **election results at different levels** (national, state, constituency).\
✔️ Comparing **party and alliance performances**.\
✔️ Analyzing **voting patterns** (EVM vs. Postal Votes).\
✔️ Identifying **top candidates** and **key battles** in the election.

---

## 📢 **Usage Instructions**

1. **Set Up the Database**

   - Run the `CREATE TABLE` scripts to initialize the database.

2. **Insert Election Data**

   - Populate the tables with real election data.

3. **Execute Queries**

   - Run the SQL queries to extract insights.

4. **Modify Queries as Needed**

   - Adjust filters (`WHERE` conditions) for **specific states, constituencies, or parties**.

---

## 🔍 Future Enhancements
- 🌟 **Data visualization** using Power BI or Tableau for intuitive insights.
- 🌐 **Advanced analytics**, including forecasting and segmentation.
- ⚡ **Performance optimization** of SQL queries for faster analysis.
- 📊 **Visualization of election results using dashboards.**
- 🔍 **Advanced analytics on voter turnout and swing percentages.**
- 🏙 **City-wise and district-wise breakdowns.**
- 🌐 **Integration with live election result updates.**

## 👥 Contributing
Contributions are welcome! Feel free to fork the repository and submit pull requests with improvements.

## 🔧 How to Use
1. **Clone the repository:**
   ```sh
   git clone https://github.com/dasarijashwanth/Indian-Elections-2024-SQL.git
   ```
2. **Import the dataset** into your SQL environment.
3. **Run the provided SQL queries** in sequence to analyze and visualize the election data.

## 📚 License
This project is licensed under the **MIT License**. See the LICENSE file for details.

For more insights, connect with me on **LinkedIn**. 🚀
