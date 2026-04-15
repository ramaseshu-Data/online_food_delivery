# Online Food Delivery System Ontology

This project presents an **Online Food Delivery System Ontology** developed using **Protégé and OWL 2**. It models the core components of a food delivery platform, including customers, restaurants, delivery agents, orders, menu items, payments, and addresses.

---

## 📌 Project Overview

The ontology represents a real-world food delivery system by defining:

- Structured **class hierarchy**
- Relationships using **object properties**
- Attributes using **data properties**
- Sample data through **individuals**
- Logical rules like **disjointness** and **cardinality restrictions**
- Validation using **HermiT Reasoner**
- Data retrieval using **SPARQL queries**

---

## 🧱 Class Hierarchy

- **Person**
  - Customer
  - DeliveryAgent
- **Restaurant**
- **Order**
- **MenuItem**
- **Payment**
- **Address**

---

## 🔗 Object Properties

- `placesOrder` (Customer → Order)  
- `hasAddress` (Customer → Address)  
- `containsItem` (Order → MenuItem)  
- `hasPayment` (Order → Payment)  
- `preparedBy` (Order → Restaurant)  
- `deliversOrder` (DeliveryAgent → Order)  

---

## 🧾 Data Properties

- `personName` (string)  
- `restaurantName` (string)  
- `itemName` (string)  
- `orderDate` (dateTime)  
- `paymentAmount` (decimal)  
- `addressLine` (string)  

---

## 👥 Sample Individuals

- Customers: Asha Reddy, Rohan Kumar  
- Delivery Agents: Vikram Singh, Neha Sharma  
- Restaurants: Spice Hub, Pizza Point  
- Orders: Order_001, Order_002  
- Items: Chicken Biryani, Veg Pizza  
- Payments: 450.00, 300.00  
- Addresses: Hyderabad locations  

---

## ⚙️ Ontology Constraints

### Disjointness
Ensures separation between unrelated classes (e.g., Customer ≠ DeliveryAgent)

### Cardinality Restriction
- Each **Order has exactly one Payment**

---

## 🧠 Reasoning

Validated using **HermiT Reasoner**:
- No inconsistencies found  
- All constraints satisfied  
- Ontology is logically correct  

---

## 🔍 SPARQL Queries

Implemented queries to:

1. List all customers  
2. Retrieve customers and their orders  
3. Get orders with items  
4. Find delivery agents and deliveries  
5. Validate payment constraint  
6. Retrieve customers with addresses  

---

## 🛠️ Tools Used

- Protégé  
- OWL 2  
- RDF/XML  
- HermiT Reasoner  
- SPARQL  

---

## 📁 File

- `online_food_delivery.owl` – Ontology file  

---

---

## 📖 Conclusion

This project demonstrates how semantic web technologies can model a real-world system using ontology design, logical constraints, reasoning, and query-based validation.
