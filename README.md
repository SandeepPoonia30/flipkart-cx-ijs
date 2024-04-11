# Flipkart CX IJS Support POC

A web application demonstration replacing Excel-based incident management.  Features incident resolution/disposition selection, status tracking, and Flipkart agent response logging. Built with Asp.net Nextjs (frontend), Asp.net Core Web API (backend), and MS SQL 2019 (database).

[https://www.youtube.com/watch?v=t1KYfw3hiUU](https://i9.ytimg.com/vi_webp/t1KYfw3hiUU/mq3.webp?sqp=CJSA4bAG-oaymwEmCMACELQB8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGGUgZShlMA8=&rs=AOn4CLCO91rhF97wmuH6MpfKEPPCzDvgwg)

## High-Level Overview

**1. Customer Input:** The code begins by collecting customer input. This includes:

   - Item value
   - Issue Type and Issue
   - Presence/absence of product
   - Presence/absence of product image

**2. Determining Resolution and Disposition:** Based on the customer input, the code uses decision logic (e.g., if/else statements or switch cases) to determine the appropriate:

   - Resolution (how to solve the issue)
   - Disposition (final status of the complaint)

**3. Notes Generation:** The code generates tailored notes for the agent to copy. These notes likely include:

   - Summary of the issue
   - Steps for the agent to take
   - Pre-written text to use in communication with the customer

**4. Workflow Integration:**

   - **TOA/ACT Form:** The code determines if a TOA (Transfer of Accountability) or ACT (Act on Complaint) form needs to be filled out, likely based on the resolution and disposition. It may automatically populate some form fields.

**5. Ticket Generation:**

   - The code generates a unique ticket ID.
   - It stores relevant information in a database or tracking system, including customer details, issue description, resolution, disposition, and generated notes.

**6. Ticket Navigation:**

   - The code provides the agent the ability to easily access the ticket using its ID.

**7. Ticket Response:**

   - The agent can update the ticket, adding their response and any further actions taken.

### Example Explanation (for a specific scenario)

"Let's say a customer reports their item is damaged and its value is under a certain threshold. The code determines the resolution (e.g., refund), disposition (e.g.,resolved), and generates notes instructing the agent to process a refund. Since the value is low, no TOA/ACT form is needed. A  ticket is created, and the agent can navigate to it to issue the refund and communicate with the customer."
