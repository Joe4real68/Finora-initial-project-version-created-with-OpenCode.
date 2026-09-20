# **Product Requirements Document (PRD)**

## **Finora**

**Product Name:** Finora  
**Product Type:** Personal income and expense management app  
**Primary Audience:** Individuals, freelancers, service providers, small business owners, and anyone who wants better control over their finances  
**Core Differentiator:** Intelligent spending insights with an optional automatic tithe-tracking feature for Christians

---

## **1\. Product Overview**

Finora is a personal finance management app designed to help users understand where their money comes from, where it goes, and how much they have available.

The app allows users to record their income and expenses, monitor their financial activity, identify spending patterns, and receive useful insights about their financial behaviour.

Finora also includes an optional **Tithe Tracker** for Christian users. When enabled, the app automatically calculates 10% of recorded income and accumulates the amount until the user marks the tithe as paid.

The goal is not simply to help users record transactions, but to help them become **more aware, disciplined, and intentional with their money.**

---

# **2\. Problem Statement**

Many people, especially freelancers, service providers, small business owners, and those with irregular income, struggle to keep track of how much they earn, spend, and have left. Because spending can happen gradually without a clear picture of their finances, it is easy to overspend or make poor financial decisions without realising it until their money is almost gone.

Finora aims to solve this by providing a simple and intelligent way to track income and expenses, monitor spending patterns, and provide financial insights that encourage users to make better and more intentional spending decisions.

The app will also include an optional feature for Christians to stay consistent with their tithe. When enabled, it automatically calculates 10% of recorded income and accumulates the amount, removing the stress of manually calculating tithe from different income sources.

---

# **3\. Product Goals**

Finora should help users:

* Know exactly how much they earn.  
* Know exactly how much they spend.  
* Understand where their money goes.  
* Know their available balance.  
* Identify unhealthy or unusual spending patterns.  
* Make more intentional spending decisions.  
* Keep track of financial obligations.  
* Reduce the stress of manually calculating tithe.  
* Build better financial awareness and discipline.

---

# **4\. Target Users**

### **Primary Users**

**Freelancers and service providers**

People who receive payments from different clients and projects and may not have a fixed monthly income.

**Small business owners**

People who receive money from customers regularly and need a simple way to monitor income and expenses.

**Employees**

People with regular salaries who want better control over their personal spending.

**Students and young adults**

People learning how to manage their money and develop healthy financial habits.

### **Christian Users**

Christians who want an easier way to calculate, accumulate, and monitor their tithe alongside their regular financial activities.

---

# **5\. Core Product Features**

## **5.1 User Account**

Users should be able to create and manage their Finora account.

### **Requirements**

Users should be able to:

* Create an account.  
* Log in.  
* Log out.  
* Manage basic profile information.  
* Set their preferred currency.  
* Access their financial information privately.

---

# **6\. Dashboard**

The dashboard is the user's financial home screen.

It should provide an immediate overview without overwhelming the user.

### **Dashboard should display:**

**Available Balance**

The user's current balance based on recorded income and expenses.

**Total Income**

The amount earned within the selected period.

**Total Expenses**

The amount spent within the selected period.

**Tithe Balance**

Only displayed when the tithe feature is enabled.

**Financial Insight**

A short, useful observation based on the user's financial activity.

### **Example**

> **You've earned ₦500,000 this month and spent ₦180,000. Your spending is currently within your usual range.**

The dashboard should make it possible for users to understand their financial position at a glance.

---

# **7\. Income Tracking**

Users should be able to record every income received.

### **When adding income, users should provide:**

* Amount  
* Income source  
* Category  
* Date  
* Optional note

### **Examples**

> Client Payment — ₦150,000  
> Salary — ₦250,000  
> Freelance Project — ₦80,000  
> Business Sales — ₦50,000

Finora should automatically update the user's total income and available balance.

---

# **8\. Expense Tracking**

Users should be able to record their spending.

### **When adding an expense, users should provide:**

* Amount  
* Expense category  
* Date  
* Optional note

### **Example categories**

* Food  
* Transportation  
* Bills  
* Rent  
* Shopping  
* Entertainment  
* Business  
* Education  
* Health  
* Giving  
* Other

Users should be able to create custom categories if necessary.

---

# **9\. Transaction History**

Users should have access to a complete history of their financial activities.

Each transaction should clearly show:

* Type: Income or Expense  
* Amount  
* Category/source  
* Date  
* Note, if available

Users should be able to:

* Search transactions.  
* Filter by income or expense.  
* Filter by category.  
* View transactions by date range.  
* Edit a transaction.  
* Delete a transaction.

---

# **10\. Spending Insights**

This is one of Finora's key features.

Finora should go beyond simply recording transactions and help users understand their spending.

The app should analyse recorded financial activity and identify patterns such as:

### **High spending**

> **You've spent ₦65,000 on food this month, which is higher than your usual spending.**

### **Unusual spending**

> **Your entertainment spending this month is significantly higher than your previous months.**

### **Spending trend**

> **Your expenses have increased for the third consecutive month.**

### **Income vs spending**

> **You've spent 72% of your recorded income this month.**

### **Positive behaviour**

> **You've reduced your transportation expenses by 18% compared with last month.**

The purpose is to **inform and encourage**, not shame the user.

---

# **11\. Financial Alerts**

Finora should provide useful alerts when something deserves the user's attention.

Examples:

> ⚠️ **Spending Alert**  
> You've already spent 80% of your recorded income this month.

> 💡 **Spending Insight**  
> Your food expenses are currently higher than your average.

> 📈 **Income Update**  
> You've earned more this month than you did last month.

These alerts should be helpful rather than excessive.

Users should be able to control which notifications they receive.

---

# **12\. Tithe Tracker**

The Tithe Tracker is an **optional feature** designed primarily for Christian users.

It should not interfere with the core financial experience for users who don't want to use it.

### **Enable/Disable**

Users should be able to turn the feature on or off.

When enabled, Finora automatically calculates **10% of recorded income**.

### **Example**

User records:

> Income: ₦100,000

Finora calculates:

> Tithe: ₦10,000

The amount is added to the user's accumulated tithe.

If the user later records:

> Income: ₦50,000

The accumulated tithe becomes:

> **₦15,000**

---

# **13\. Tithe Payment**

Users should be able to mark their accumulated tithe as paid.

When they select:

> **Mark Tithe as Paid**

Finora should:

* Record the payment.  
* Show the date it was paid.  
* Reset the current accumulated tithe.  
* Keep the previous payment in the user's history.

The user should still be able to see historical tithe payments.

---

# **14\. Tithe Reset Preferences**

Users should have control over how their tithe tracking works.

Options should include:

* Weekly  
* Monthly  
* Manual

### **Manual**

The amount remains accumulated until the user manually marks it as paid.

### **Important**

The app should **not automatically erase an unpaid tithe simply because a new period has started.**

Users should always be able to see what remains unpaid.

---

# **15\. Financial Periods**

Users should be able to view their finances according to different periods.

Examples:

* Today  
* This week  
* This month  
* Last month  
* This year  
* Custom date range

This should apply to income, expenses, and relevant insights.

---

# **16\. Financial Summary**

Finora should provide users with a simple summary of their financial activity.

For a selected period, users should be able to see:

* Total income  
* Total expenses  
* Balance  
* Spending by category  
* Income by source  
* Tithe accumulated, if enabled  
* Major spending patterns

The information should be presented in a simple and understandable way.

---

# **17\. Financial Categories**

Finora should provide default categories for common income and expenses.

Users should also be able to:

* Add custom categories.  
* Rename categories.  
* Remove categories they no longer use.

The goal is to allow Finora to adapt to different lifestyles and professions.

---

# **18\. AI Financial Assistant**

Finora should eventually include an AI-powered financial assistant that can help users understand their recorded financial information.

The AI should work primarily with the user's Finora data rather than providing generic financial advice.

Users could ask:

> "How much did I spend on food this month?"

> "What category am I spending the most on?"

> "How much did I earn this month?"

> "Why is my balance lower than last month?"

> "What changed in my spending this month?"

The assistant should provide simple explanations based on the user's recorded information.

---

# **19\. Affordability / Spending Check**

One of Finora's more advanced features could allow users to check a planned expense before making it.

For example:

> **Can I afford to spend ₦100,000 on a new phone?**

Finora could consider the user's:

* Current balance  
* Recent income  
* Recent expenses  
* Spending patterns  
* Upcoming recorded expenses

It can then provide an objective financial perspective.

For example:

> **After this purchase, your available balance would be ₦85,000. Based on your recent spending, this would leave you with less room for your usual expenses.**

The feature should help users **think before spending**, rather than make decisions for them.

---

# **20\. Savings Goals**

This can be included in the initial version if it remains manageable, or introduced shortly after the MVP.

Users could create goals such as:

> Emergency Fund — ₦500,000

> New Laptop — ₦800,000

> Rent — ₦600,000

The app could show:

**₦250,000 / ₦500,000**

**50% completed**

This would extend Finora beyond tracking into financial planning.

---

# **21\. Reports**

Users should be able to review their financial performance over time.

Possible reports:

* Monthly income  
* Monthly expenses  
* Spending by category  
* Income sources  
* Tithe history  
* Balance trends

Reports should be simple enough for an everyday user to understand.

---

# **22\. Notifications**

Users may receive useful reminders such as:

* Record your recent income.  
* You haven't recorded an expense recently.  
* Your spending has increased.  
* Your tithe has accumulated.  
* Your selected tithe period is ending.  
* Monthly financial summary is ready.

Users should have the ability to manage notification preferences.

---

# **23\. User Experience Principles**

Finora should feel:

**Simple**  
Users should not need financial knowledge to understand the app.

**Clean**  
The interface should avoid unnecessary information and clutter.

**Private**  
Financial information should feel secure and personal.

**Helpful**  
Insights should help users understand their behaviour.

**Non-judgmental**  
Finora should encourage financial discipline without making users feel guilty or ashamed.

**Faith-friendly**  
Christian features should feel natural and optional rather than forcing religious elements on every user.

---

# **24\. MVP Scope**

For the first version, I recommend focusing on:

### **Essential**

1. Account creation and login  
2. Dashboard  
3. Add income  
4. Add expenses  
5. Transaction history  
6. Income and expense summaries  
7. Spending categories  
8. Basic spending insights  
9. Tithe Tracker  
10. Mark tithe as paid  
11. Tithe history  
12. Basic financial settings

### **Phase 2**

After the core product works well:

* AI Financial Assistant  
* Affordability checker  
* Savings goals  
* Advanced financial insights  
* More detailed reports  
* Custom notification settings  
* Recurring income and expenses

This keeps the certificate project **realistic while still giving Finora a compelling identity**.

---

# **25\. Key User Journey**

A typical Finora user should be able to:

**Sign up → Set up profile → Add income → Add expenses → View balance → Review spending → Receive insight → Track tithe if enabled → Mark tithe as paid → Continue tracking**

The experience should feel simple enough that recording a transaction takes only a few seconds.

---

# **26\. Success Criteria**

Finora will be considered successful when a user can:

* Quickly record income.  
* Quickly record expenses.  
* Immediately understand their available balance.  
* See where their money is going.  
* Recognise spending patterns.  
* Receive useful financial insights.  
* Easily calculate and track tithe if enabled.  
* Review their financial history.  
* Feel more informed and intentional about their spending.

---

# **27\. Product Positioning**

### **One-line description**

> **Finora is a smart personal finance tracker that helps you understand your income, control your spending, and manage your money intentionally.**

### **Christian-focused description**

> **Finora helps you manage your money wisely while giving you an optional, simple way to track your tithe and practise faithful financial stewardship.**

### **Possible tagline**

> **Know your money. Manage it wisely.**

Other possibilities:

> **Track it. Understand it. Manage it.**

> **Your money, made clearer.**

> **Earn. Spend. Give. Know.**

I would keep **"Know your money. Manage it wisely."** as the strongest general-purpose direction for now.

---

## **28\. Future Vision**

Finora can eventually grow beyond a basic income and expense tracker into a personal financial companion that helps users:

**Track → Understand → Plan → Decide → Improve**

The long-term vision is for Finora to help people develop a clearer relationship with their money, regardless of whether they are salaried employees, freelancers, business owners, students, or Christians using the optional stewardship features.

**The key principle:** Finora should not simply tell people what they did with their money. It should help them **understand their financial behaviour and make more intentional decisions going forward.**

