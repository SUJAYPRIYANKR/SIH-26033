# Smart India Hackathon Workshop
# Date:29/10/2026
## Reference Number:26016948
## Name:SUJAY PRIYAN K R

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
KisanDirect is a digital marketplace that connects farmers and FPOs directly with consumers and bulk buyers, so the produce reaches the buyer without passing through several middlemen. Farmers list their crops on the app, buyers order straight from them, and the price is shown clearly, including the farmer’s share, the delivery cost and a small platform fee.

To make this work for small farmers, the platform also handles logistics. Produce is collected at local FPO hubs, graded and packed, and then sent out in combined loads. This keeps delivery cost low and means a farmer doesn’t have to arrange transport alone.

AI is used in two places. A demand forecasting model uses mandi prices, weather and past orders to tell farmers what is likely to sell and at what price. A route optimization model plans the best pickup and delivery routes, so vehicles run full and produce reaches buyers fresh.
## Proposed Solution
KisanDirect is a mobile and web marketplace where farmers and FPOs list their produce and consumers, restaurants, retailers and bulk buyers order from them directly. The farmer sets a base price with the help of live mandi rates shown in the app. The buyer sees where the produce comes from, what it costs and when it will arrive.

Farmer/FPO app: simple, works in regional languages, supports voice input, and runs on low data. Farmers upload a photo, quantity and expected harvest date.
Buyer app: consumers can buy in small quantities, bulk buyers can place scheduled or contract orders.
Logistics layer: local collection points (village hubs run by FPOs) where produce is gathered, graded and sent out in combined loads, so a single farmer doesn’t have to arrange transport.
<img width="2600" height="1506" alt="image" src="https://github.com/user-attachments/assets/d02da33a-9f4c-4545-b1ef-fda9f3e36fe4" />


How it addresses the problem

Today produce passes through several hands (local trader, commission agent, wholesaler, retailer), and each one adds a margin. Farmers often get only 25-40% of what the consumer pays. By connecting the farmer to the buyer directly and using pooled transport, we cut out most of these steps. What’s left is a small platform fee and the transport cost, so the farmer earns more and the consumer pays less at the same time.

Innovation and uniqueness

Demand forecasting that tells farmers what to grow and sell, not just where to sell.
Pooled delivery using route optimization, so small farmers can reach city buyers cheaply.
Price transparency: the app shows how the final price breaks down (farmer share, transport, platform fee).
Works for low-literacy and low-connectivity users through voice, icons and an SMS/WhatsApp fallback.
Built around FPOs, so the group handles grading, packing and trust instead of each farmer doing it alone.
## Technical Approach
Technologies to be used

Frontend: Flutter for the Android app, React for the web dashboard.
Backend: Node.js (Express) or Python (FastAPI), with REST APIs.
Database: PostgreSQL for orders and users, MongoDB for listings, Redis for caching.
AI/ML: Python with scikit-learn, Prophet or LSTM (TensorFlow) for demand and price forecasting. Google OR-Tools for route optimization.
Maps and location: Google Maps API or OpenStreetMap.
Data sources: Agmarknet / data.gov.in for mandi prices, IMD for weather.
Payments: UPI / Razorpay with escrow style payout to farmers after delivery.
Language and voice: Bhashini API for regional language translation and speech.
Hosting: AWS or any cloud with Docker for deployment.
## Feasibility and Viability
Feasibility

Built on existing technology: apps, UPI payments, maps and route optimization tools are all readily available.
Public data like Agmarknet and data.gov.in can be used to train the price and demand forecasting model.
FPOs and village networks already exist, so we don’t need to build a farmer base from scratch.
A small commission of 2-4% keeps the platform sustainable and is far lower than middlemen margins.

Challenges and risks

Farmers with low digital literacy and weak internet
Spoilage of perishable produce during transport
Farmers depending on local traders for loans
Getting enough buyers and sellers in one area at the start
Quality disputes between farmers and buyers

Strategies to overcome them

Voice-based, regional-language app with SMS/WhatsApp backup
Village hubs for grading and packing, with cold storage tie-ups
Advance payment or small credit options through FPOs and cooperative banks
Pilot launch in one district with 3-4 crops
Grading at hubs, ratings, and escrow payments to build trust
## Impact and Benefits
Potential impact on the target audience

Farmers/FPOs: a bigger share of the final price, quicker payments, and better planning on what to grow and when to sell.
Consumers: fresher produce at lower prices, with clear information on where it came from.
Bulk buyers: steady supply and the option of contract orders.
Rural youth: jobs as hub operators, packers and delivery partners.

Benefits

Social: more bargaining power for small farmers, digital inclusion in villages, local employment.
Economic: higher farmer income, lower consumer prices, less cost lost to middlemen.
Environmental: less food waste through better demand matching, and fewer wasted trips through route optimization.

## Research and References
Link: https://www.rbi.org.in/scripts/bs_viewbulletin.aspx?id=18527
https://www.drishtiias.com/daily-updates/daily-news-analysis/farmers-earning-in-agri-produce-rbi
https://www.rbi.org.in/scripts/BS_ViewBulletin.aspx?Id=18527
https://epubs.icar.org.in/index.php/IJAgS/article/download/118588/45740/336847
