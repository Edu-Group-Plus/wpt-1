# Senior WordPress & PHP Developer Test Assignment

---

## Objective

Build a custom WordPress plugin to manage a **Dynamic User Scoring System** integrated with WooCommerce. The scoring system should track user activity and assign scores based on specific actions. This will evaluate your understanding of database interactions, WooCommerce integration, and backend logic.

### Key Features

1. **User Score Tracking**:
   - Implement a custom database table (using the WordPress database API) to store user scores.
   - Track scores for the following actions:
     - Placing an order (different scores based on the total value of the order).
     - Leaving a product review.
     - Logging in (limit to once per day).

2. **Admin Panel**:
   - Create a custom admin menu to:
     - View all users and their scores.
     - Reset a user’s score.
     - Add or deduct points manually for a user.
     - Backfill scores for existing orders of a user (recalculate scores based on order history).
   - Use custom WP_List_Table for displaying users and scores in the admin panel.

3. **Frontend Display**:
   - Show the user’s current score on their account page.
   - Display a leaderboard of top 10 users with the highest scores on a custom page (e.g., `/leaderboard`).

4. **WooCommerce Integration**:
   - Automatically assign scores based on WooCommerce order value:
     - 1 point for every $10 spent.
     - Bonus 50 points for orders over $500.
   - Add a notification to the user’s order confirmation email with the number of points earned.

5. **Environment Setup**:
   - Use **Lando** for local development.
   - Include a `lando.yml` file for setting up the WordPress environment.
   - Provide clear instructions for starting the project using Lando.

6. **Optional MVC Approach**:
   - You may choose to structure the plugin using an MVC format for better organization and modularity. This can be done using either **Timber** (Twig templates for views) or the **Roots.io ecosystem** (e.g., Sage for templating). Include detailed instructions in your `README.md` if you opt for this approach.

---

## Deliverables

1. **Codebase**:
   - WordPress plugin for the scoring system.
   - Admin panel and database schema creation.

2. **Documentation**:
   - A `README.md` file with:
     - Installation and setup instructions.
     - Steps to run the project using Lando.
     - Explanation of the technical approach.
     - Any assumptions made.

3. **Submission**:
   - Clone this repository as a private repository on your GitHub account.
   - Commit your work to your private repository.
   - Add viraj@exampapersplus.co.uk as a collaborator to grant access.
   - Submit the link to your private repository.

---

## Notes on Deadlines and Features

- The suggested deadline for this assignment is **1 week**. However, we understand that schedules can vary, so the timeline is flexible.
- While it is encouraged to implement all the features outlined in the assignment, it is not mandatory to complete every single feature. Prioritize quality over quantity and focus on demonstrating your expertise and problem-solving skills.
