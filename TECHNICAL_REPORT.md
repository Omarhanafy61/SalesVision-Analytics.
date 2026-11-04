# SalesVision Analytics
## Interactive Sales Performance Dashboard
**Technical Project Report — Web Development for Data Dissemination**

### 1. Project overview
SalesVision Analytics is a responsive, interactive website that presents a simulated retail sales dataset through key performance indicators (KPIs), charts, a transaction table and category/region filters. Its purpose is to transform raw transaction records into accessible information that helps a viewer understand sales performance.

### 2. Objectives
- Organize sales records in a structured CSV dataset.
- Calculate total revenue, total profit, units sold and best-selling product.
- Visualize monthly revenue, category contribution, product volume and payment-method revenue.
- Allow users to filter by product category and sales region.
- Present underlying transactions and allow filtered records to be exported.
- Publish the responsive website online using GitHub Pages.

### 3. Dataset description
The project uses 72 simulated sales transactions dated January through December 2025. Each record contains an order ID, date, product ID and name, category, region, quantity, unit price, revenue, cost, profit and payment method. The dataset is synthetic and must not be represented as actual company performance.

Calculation methods: Revenue = quantity sold × unit price. Cost = quantity sold × unit cost. Profit = revenue − cost. Dashboard totals are calculated by summing relevant transaction values after active filters are applied. The best-selling product is determined by total units sold.

### 4. Technologies
- HTML5: semantic page structure and accessible sections.
- CSS3: custom visual styling and responsive adjustments.
- Bootstrap 5: responsive grid and layout utilities.
- JavaScript: CSV loading, calculations, filtering, table rendering and event handling.
- Chart.js: line, doughnut, bar and pie visualizations.
- CSV: portable structured dataset used by the website.
- Visual Studio Code and Live Server: development and local testing.

### 5. Dashboard components
The KPI cards show total revenue, total profit, units sold and the best-selling product. Four visualizations communicate different aspects of the dataset:
- Monthly revenue (line chart): shows revenue trends across the twelve months.
- Revenue by category (doughnut chart): compares category contributions.
- Top products by units sold (bar chart): compares product volume.
- Revenue by payment method (pie chart): shows transaction value distribution.

### 6. Interactivity and processing
The category and region dropdowns filter the original records. The dashboard recalculates KPIs, updates charts and redraws the transaction table. Transaction search narrows visible rows. The export control downloads the currently filtered records as a CSV file.

### 7. Responsive design and accessibility
Bootstrap's grid and custom CSS breakpoints adapt the layout to desktop, tablet and mobile screens. Semantic headings and sections, form labels, and responsive tables improve usability. A production version could further improve accessibility by adding equivalent detailed data tables for every chart.

### 8. Data transparency and limitations
Source: simulated teaching dataset generated for this project. Period covered: January–December 2025. Number of records: 72. Currency: Egyptian pounds (EGP). The records are illustrative and do not establish real market trends. The sample is relatively small, uses a limited set of products and regions, and does not include returns, taxes, shipping charges, discounts as separate fields or customer-level behavior. Conclusions should therefore be limited to this sample.

### 9. Testing checklist
- [ ] Confirm sales_data.csv loads when the site is served through Live Server.
- [ ] Check initial KPI values against manual calculations from the CSV.
- [ ] Select each category and region and verify that KPIs, charts and table update.
- [ ] Search for an order ID and a product name in the transaction table.
- [ ] Export filtered CSV and verify that it contains only matching records.
- [ ] Test layout, charts and table on desktop, tablet and mobile widths.
- [ ] Check browser console for errors before publishing.

### 10. Deployment
The website is a static frontend and can be hosted on GitHub Pages. Keep index.html, styles.css, app.js and sales_data.csv in the same published directory. Configure repository Settings → Pages to deploy from the main branch and root folder. Test the published URL to confirm the CSV loads and all filters and charts work.

### 11. Conclusion
SalesVision Analytics demonstrates the data dissemination workflow: structured data, calculation of indicators, visual communication, interactive exploration, responsive presentation and online publication. The dashboard is designed to meet the project brief while clearly disclosing that its dataset is simulated.
