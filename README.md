# 🏠 Airbnb Analysis Dashboard (Power BI)

An **end-to-end Power BI analytics solution** delivering actionable insights into Airbnb listings performance, revenue drivers, and market dynamics. Built as a solo BI project covering data prep, modeling, DAX, and dashboard design.

---

## 🎯 Business Problem

Regional teams lacked a **unified view of revenue and performance** across cities and listing types.

**Key questions addressed:**
- Where is revenue concentrated?
- Which listing attributes drive bookings?
- How can pricing be optimized without hurting occupancy or guest satisfaction?

**Goal:** Build a **self-service Power BI dashboard** to support pricing strategy, host acquisition, and market prioritization.

---

## 🗂️ Data Architecture

**Fact & Dimension Model (Listing-Day Granularity):**
- **Listings:** city, room type, price, beds, bedrooms, bathrooms, response rate, guest favourite
- **Hosts:** host tenure, superhost flag, primary city
- **Sales:** booking date, nights booked, revenue per stay
- **Dimensions:** city & date for time intelligence

**Coverage:** 12 months of completed stays aligned to reporting cycles.

---

## 🛠️ Data Cleaning & Feature Engineering

- **Schema standardization:** cleaned prices, dates, numerics
- **Feature engineering:** price categories (Low/Mid/High), host tenure buckets, guest favourite flags
- **Quality control:** handled missing values, standardized room types, removed duplicates
- **Integration:** joined listings, hosts, and sales; removed orphan records
- **Outlier filtering:** excluded test listings, extreme prices, negative revenue

---

## 📊 Dashboard Structure

### 1️⃣ Overview (Executive View)
- **$16M** total sales (12 months)
- **$183** average room price
- **44K** active hosts
- Revenue concentration by city (Tokyo & Sydney lead)

### 2️⃣ Room Analysis (Supply Intelligence)
- Pricing by room type
- Bedroom & bathroom distribution
- Inventory mix and configuration insights

### 3️⃣ Sales Deep-Dive (Revenue Drivers)
- Host tenure vs revenue trends
- Top hosts by sales
- Decomposition tree: Room Type → Price Category → Guest Favourite

---

## 🔍 Key Insights

- **Revenue concentration:** Tokyo & Sydney contribute ~35% of total sales
- **Supply imbalance:** High-priced listings dominate inventory (52K vs 4K low-priced)
- **Core segment:** 2-bed, 1–2 bedroom listings drive the highest ROI
- **Host lifecycle:** Revenue peaks at 2–5 years tenure, then plateaus
- **Guest experience upside:** Non-guest-favourite listings still generate strong revenue → quality improvements unlock pricing power

---

## 💡 Business Impact

- Replaced fragmented Excel reporting with a **single interactive dashboard**
- Enabled **self-service analytics** for pricing, supply, and host strategy
- Quantified revenue drivers across cities, room types, and host tenure
- Estimated **5–10% revenue uplift** in priority markets through optimized pricing & mix

---

## 🔮 Future Enhancements

- Booking-level occupancy analysis  
- Demand forecasting & seasonality trends  
- Predictive pricing models  
- Row-level security by region/role  
- Automated refresh & scalable extensions  

---

## 🧑‍💻 Tech Stack

- **Power BI** (DAX, data modeling, report design)
- **Star schema** with time intelligence
- End-to-end BI workflow
