# Smart Inventory Management System

## Introduction
The goal of this challenge is to demonstrate your expertise in software design, development, and deployment by building a scalable smart inventory management system. This system should allow users to manage their inventory items efficiently, including operations to add, view, update, and delete items. 
The key core functions include item management, supplier management, user management, and reporting and analytics.

## Data Persistence
Flexible Persistence Layer: Implement a persistence layer using a convenient database technology. Ensure the system is designed flexibly to allow switching to another database technology with minimal impact. Design an appropriate database schema covering all necessary inventory item details.

## Core Functions

### 1) Item Management

Manage items by adding, updating, viewing, and deleting them. Automatically update inventory stock levels when items are modified.

Benefit: Streamlines item processing and improves accuracy.

Inventory Categorization

Categorize inventory items, enabling users to search and filter based on categories.

Benefit: Makes it easier to manage and locate items.

### 2) Supplier Management

Create, update, and view supplier details, and link suppliers to inventory items.

Benefit: Streamlines procurement and keeps supplier information up-to-date.

### 3) User Management

Manage user accounts by adding, updating, viewing, and deleting user information. Implement role-based access control.

Benefit: Ensures secure and efficient management of user permissions.

### 4) Reporting and Analytics

Develop a module to generate reports on inventory levels, sales, and reordering needs. Use visual tools to present data clearly.

Benefit: Provides insights for informed decision-making.

## Database Design 
### 1. Tables and Relationships
- Items Table
	- Purpose: Store details about inventory items. 
	- Columns: 
		- `ItemID` (Primary Key) 
		- `ItemName` 
		- `Quantity` 
		- `CategoryID` (Foreign Key) 
		- `SupplierID` (Foreign Key) 
- Categories Table
	- Purpose: Categorize inventory items.
	- Columns: 
		- `CategoryID` (Primary Key) 
		- `CategoryName` 
- Suppliers Table
	- Purpose: Store details about suppliers. 
	- Columns: 
		- `SupplierID` (Primary Key) 
		- `SupplierName` 
		- `ContactInfo` 
- Users Table 
	- Purpose: Manage user information. 
	- Columns: 
		- `UserID` (Primary Key) 
		- `UserName` 
		- `Role` 
		- `Email` 
		- `Password`