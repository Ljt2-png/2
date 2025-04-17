# # Requisition System Code Analysis

## Software Design Principle Implementation

### Single Responsibility Principle
In the `RequisitionSystem` class, each method focuses on a specific task. For example, the `collect_staff_info` method is responsible for collecting staff information, the `collect_requisition_items` method is responsible for collecting requisition item information, the `approve_requisition` method is responsible for approving requisitions, and the `display_requisition` method is responsible for displaying requisition information. This design makes the function of each method clear, improving the readability and maintainability of the code. When you need to modify or extend a certain function, you only need to focus on the corresponding method.

### Open - Closed Principle
The code is open for extension and closed for modification. For example, if you want to add a new approval rule, you only need to add new logic in the `approve_requisition` method without modifying other methods. This allows the system to be extended without affecting existing functions.

## Code Functionality
This code implements a simple requisition system with the following functions:
1. Collect staff information, including date, staff ID, and staff name, and generate a unique requisition ID.
2. Collect requisition item information, including item name and price, and calculate the total price.
3. Approve the requisition based on the total price. If the total price is less than 500, the requisition is approved, and an approval reference number is generated.
4. Display requisition information, including date, requisition ID, staff ID, staff name, total price, requisition status, and approval reference number.

## Usage
Run the `requisition_system.py` file and follow the prompts to enter relevant information to complete the requisition process. You can choose whether to submit another requisition.
