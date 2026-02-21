Operational-Feasibility-Analysis : Improving Batch Assignment Logic in a Grocery Delivery Platform

(A) Executive Summary : During my experience working as an independent shopper on a gig-based grocery delivery platform, I observed a recurring operational inefficiency related to late-stage batch assignment. Orders were often released close to store closing time, sometimes with large item quantities. In several cases, the available time was insufficient to complete the order, resulting in cancellations, wasted effort and customer dissatisfaction. This project analyzes the issue from a business operations perspective and proposes a feasibility validation approach to improve reliability and efficiency.

(B) Business Problem : The batch assignment process does not appear to consistently validate whether an order can realistically be completed within remaining store operating hours.

(C) Resulting Challenges:
1. Shopper time and effort wasted
2. Order cancellations and refunds
3. Customer dissatisfaction
4. Operational inefficiencies for the platform  

(D) Current Process Flow (Observed)
Customer Order Placed -> Batch Created by System -> Shopper Accepts Order -> Store Closing Approaches -> Incomplete Order / Cancellation

Key Gap: No visible feasibility validation before batch release.

(E) Proposed Improved Process Flow
Customer Order Placed -> Batch Created -> Store Closing Time Check -> Estimated Completion Time Calculated

If Feasible -> Release Batch
If Not -> Hold / Delay Batch

Expected Improvement:
1. Higher completion rate
2. Better shopper productivity
3. Improved customer trust

(F) Simple Feasibility Calculation Model
Estimated Completion Time = (Item Count × Avg Pick Time per Item) + Estimated Checkout Time + Safety Buffer
Example:

<img width="257" height="143" alt="Screenshot 2026-02-21 at 12 52 31 AM" src="https://github.com/user-attachments/assets/0d4c8cc6-932a-4e9b-8c0e-f7b8722db480" />

If the store closes in 30 minutes, the batch should not be released.
This type of validation helps ensure operational feasibility before assignment.

(G) Stakeholder Impact Analysis
1. Shopper
- Reduced wasted effort
- More predictable earnings
- Improved work experience

2. Customer
- Fewer cancellations
- Better reliability
- Increased trust in platform

3. Platform / Business
- Lower refund costs
- Reduced support load
- Improved operational efficiency
- Stronger customer retention

(H) Risk Considerations

<img width="731" height="157" alt="Screenshot 2026-02-21 at 12 56 23 AM" src="https://github.com/user-attachments/assets/c1c22924-e174-410a-845b-6bdad3e7e27c" />


(I) Recommendations: 
1. Introduce Completion Feasibility Validation : Before releasing batches, validate whether the estimated completion time fits within remaining store operating hours.
2. Implement Dynamic Cut-Off Rules : Automatically limit batch releases close to store closing time with flexibility based on order size and historical performance.
3. Integrate Real-Time Store Hours Data : Ensure store operating hours are accurate and dynamically updated to support better decision-making.
4. Use Historical Performance Metrics : Leverage past pick-time data and checkout durations to improve prediction accuracy.
5. Monitor KPIs Post-Implementation : Order completion rate, Shopper cancellation rate, Refund frequency, Customer satisfaction indicators, Continuous monitoring will help refine the process.

(J) Business Value Potential: 
1. Increase order completion reliability
2. Improve shopper productivity and retention
3. Enhance customer experience
4. Reduce operational costs
5. Strengthen platform reputation

(K) Limitations: This analysis is based on field observation as a platform user and independent contractor. No internal operational data was accessed.
Recommendations are conceptual and intended to demonstrate structured business analysis thinking.

This project reflects how real-world operational observations can be translated into structured business analysis insights.
It demonstrates practical problem identification, stakeholder awareness and solution-oriented thinking aimed at improving operational efficiency and customer experience.
