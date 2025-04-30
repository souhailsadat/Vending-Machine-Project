# Vending Machine Project

A simple drink vending machine built with EJB (Enterprise JavaBeans) and deployed on GlassFish (Java EE server). Designed for a software architecture course, this project demonstrates component-based design with three core components:

1. Caisse component: Handles money (coins) and gives change
2. Stock component: Manages drink inventory (both for customers and restocking)
3. Command component: Controls the machine, connecting the cash and stock parts

```mermaid
flowchart LR
    ClientGui-->CommandeEjb
    CommandeEjb-->CaisseEjb
    CommandeEjb-->StockEjb
