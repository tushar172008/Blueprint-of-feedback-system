# Threadline Customer Feedback

Threadline is a customer feedback website concept for small businesses, inspired by the review experiences found on larger shopping platforms such as Amazon and Myntra. It gives a business a branded place to collect customer opinions about products and service, understand satisfaction, and use feedback to improve what it offers.

## What the website includes

- A customer feedback form with a one-to-five-star rating, product name, category, fit, written comments, and up to two photos.
- A store dashboard showing review totals, average rating, recent activity, rating distribution, and a 14-day trend.
- A PDF export for a customer satisfaction report.
- A responsive Threadline storefront and an animated product presentation.

## Current limitations

This project currently consists of `index.html`. Review submission and the staff dashboard expect a signed-in environment that provides the `claude` user, database, and download services. Opening the page in a regular browser does not provide those services, so submitting reviews and using the live dashboard will not work unless the page is hosted in a compatible environment.

The current page does not yet let a business edit an existing review or search and filter reviews by business/brand name or year. Those are useful next features for a small-business feedback system, but they need to be implemented along with suitable database fields and access controls before being advertised as available.

## Run locally

You only need a modern web browser and Visual Studio Code. There is no package installation or build step for the current single-file page.

1. Open this project folder in Visual Studio Code.
2. Open the **Extensions** view (`Ctrl+Shift+X`).
3. Search for **Live Server** by Ritwick Dey and install it.
4. In the Explorer, right-click `index.html` and choose **Open with Live Server**. Alternatively, open `index.html` and select **Go Live** in the status bar.
5. The page opens in your browser. Save changes in VS Code and Live Server will refresh the page.

You can also open `index.html` directly in a browser to inspect the page. Live Server is more convenient while developing. An internet connection is needed for the fonts and third-party JavaScript libraries loaded from CDNs.

## Before using it for a real business

Connect the form and dashboard to a real backend with authentication and database access. Store business or brand name and review year (or derive the year from a reliable submission timestamp), then add staff-only editing and search/filter controls. Protect customer data and uploaded photos with appropriate permissions and retention rules.
