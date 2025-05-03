

# <div align="center">🌿 UrbanFood 🌿</div>

<div align="center">
  
  ![Database GIF](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3o3M205eHY0Nno5YjBkNm84N2hjamRhMzAyazFoZXExNXU1NDh3NiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/sRFEa8lbeC7zbcIZZR/giphy.gif)

  ### <em>✨ Fresh from Farm to Table: Connecting Urban Farmers with Conscious Consumers ✨</em>
  
  [![GitHub stars](https://img.shields.io/github/stars/MrVinzSL/UrbanFood?style=social)](https://github.com/MrVinzSL)
  [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
  [![Status](https://img.shields.io/badge/Status-Active-success.svg)](https://github.com/MrVinzSL)
  
</div>

<p align="center">
  <a href="#-project-overview">Overview</a> •
  <a href="#-technical-architecture">Architecture</a> •
  <a href="#-database-components">Database</a> •
  <a href="#-technologies-used">Technologies</a> •
  <a href="#-development-team">Team</a> •
  <a href="#-demo">Demo</a>
</p>

## 📋 Project Overview

<div align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMGU1OWJiM2JkMjMzODFmZmI2ZGM5MGM5NTUzOTkwM2JmZTY0NWMzZCZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/3oKIPEqDGUULpEU0aQ/giphy.gif" width="400px" alt="Project Animation">
</div>

Welcome to **UrbanFood** - a modern e-commerce platform that connects urban farmers and local producers directly with consumers who value fresh, locally made goods. Our platform facilitates the trade of fruits, vegetables, dairy, baked items, and handmade crafts within urban communities.

> *"Building bridges between urban agriculture and conscious consumption."*

<details>
<summary>📊 Key Features</summary>
<br>

- **Direct Farm-to-Consumer Sales**: Eliminating middlemen for fresher products and better prices
- **Local Product Verification**: Ensuring authenticity of locally produced goods
- **Sustainable Packaging Options**: Reducing environmental impact
- **Community Building Tools**: Connecting like-minded producers and consumers
- **Integrated Delivery System**: Optimizing local logistics

</details>

<div align="center">
  
  ![Farm to Table](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExY2MzMGQ0MWI5NTkzNTM1YjYyNDgyNDc5YWQ5YjM0ODVjNzQ5ZjZlNSZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/l0MYsynHCr18CW26Q/giphy.gif)
  
</div>

## 🛠️ Technical Architecture

<div align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNGY5ODY3NDA5YTNiM2NhZDA3OGJiYzIzNGRhNGI5ZDdmNGU5YWJmZCZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/26tn33aiTi1jkl6H6/giphy.gif" width="500px" alt="Database Animation">
</div>

As database developers, our primary goal was to design a robust, scalable system to manage the entire e-commerce workflow. We implemented a **hybrid database approach**:




- **Oracle Database**: For structured transactional data, ensuring data integrity and business logic encapsulation through PL/SQL
- **MongoDB**: For unstructured content like product reviews and customer feedback

## 🗄️ Database Components

<div align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3o3M205eHY0Nno5YjBkNm84N2hjamRhMzAyazFoZXExNXU1NDh3NiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/xTiTnxpQ3ghPiB2Hp6/giphy.gif">
</div>

### 🔶 Oracle Database Entities

<table>
  <tr>
    <td width="50%">
      <h4>📊 Supplier</h4>
      <ul>
        <li>CRUD procedures for supplier management</li>
        <li>Trigger for audit trail</li>
        <li>Secure login function</li>
      </ul>
    </td>
    <td width="50%">
      <h4>👥 Users</h4>
      <ul>
        <li>User management procedures</li>
        <li>Authentication system</li>
        <li>User activity logging</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>
      <h4>🛒 Product</h4>
      <ul>
        <li>Complete product lifecycle management</li>
        <li>Inventory tracking</li>
        <li>Category management</li>
      </ul>
    </td>
    <td>
      <h4>💳 Payment</h4>
      <ul>
        <li>Transaction processing</li>
        <li>Payment retrieval by ID or user</li>
        <li>Audit trail for financial records</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>
      <h4>📝 Orders</h4>
      <ul>
        <li>Order creation and tracking</li>
        <li>Stock level management triggers</li>
        <li>Order analytics procedures</li>
      </ul>
    </td>
    <td>
      <h4>🚚 Delivery</h4>
      <ul>
        <li>Delivery status tracking</li>
        <li>Delivery audit system</li>
        <li>Location-based assignments</li>
      </ul>
    </td>
  </tr>
</table>

### 📊 Entity Relationship Diagram

mermaid
erDiagram
    SUPPLIER ||--o{ PRODUCT : supplies
    USERS ||--o{ ORDERS : places
    PRODUCT ||--o{ ORDERS : contains
    ORDERS ||--|| PAYMENT : has
    ORDERS ||--|| DELIVERY : requires


## 💻 Technologies Used

<div align="center">
  
  <a href="https://www.java.com/">
    <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  </a>
  <a href="https://www.oracle.com/database/technologies/appdev/plsql.html">
    <img src="https://img.shields.io/badge/PL/SQL-F80000?style=for-the-badge&logo=oracle&logoColor=white" alt="PL/SQL" />
  </a>
  <a href="https://www.mongodb.com/">
    <img src="https://img.shields.io/badge/NoSQL-4DB33D?style=for-the-badge&logo=mongodb&logoColor=white" alt="NoSQL" />
  </a>
  <a href="https://reactjs.org/">
    <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  </a>
  
</div>

<details>
<summary>💡 Technology Stack Details</summary>
<br>

mermaid
graph TD
    A[Front-End] -->|React| B[UI Components]
    A -->|API Calls| C[Back-End]
    C -->|Java| D[Business Logic]
    D -->|Query| E[Data Layer]
    E -->|PL/SQL| F[Oracle DB]
    E -->|Queries| G[NoSQL DB]


| Technology | Purpose | Features Used |
|------------|---------|---------------|
| Java | Backend Development | REST APIs, Data Processing |
| PL/SQL | Database Programming | Stored Procedures, Triggers, Functions |
| NoSQL | Unstructured Data | Document Storage, Flexible Schema |
| React | Frontend Interface | Component-Based UI, State Management |

</details>

## 🧑‍💻 Development Team

<div align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExODUzMmRkODA3NWIxYWM3YjkzN2Y5YmQ2ZGVlZmE3ZmU2M2JjZmZkZiZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/dSetNZo2AJfptAk9hp/giphy.gif" width="400px" alt="Team Animation">
</div>

<div align="center">

### 🌟 Our talented team of database developers from NIBM 🌟

</div>

<table align="center">
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/BIMSARA-COHNDSE242F--047-blueviolet?style=for-the-badge&logo=academia&logoColor=white" alt="BIMSARA"/></td>
    <td align="center"><img src="https://img.shields.io/badge/ISURA-COHNDSE242F--048-blueviolet?style=for-the-badge&logo=academia&logoColor=white" alt="ISURA"/></td>
  </tr>
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/RAVINDU-COHNDSE242F--049-blueviolet?style=for-the-badge&logo=academia&logoColor=white" alt="RAVINDU"/></td>
    <td align="center"><img src="https://img.shields.io/badge/JANINDU-COHNDSE242F--064-blueviolet?style=for-the-badge&logo=academia&logoColor=white" alt="JANINDU"/></td>
  </tr>
  <tr>
    <td align="center"><img src="https://img.shields.io/badge/JITHMITHA-COHNDSE242F--065-blueviolet?style=for-the-badge&logo=academia&logoColor=white" alt="JITHMITHA"/></td>
    <td align="center"><img src="https://img.shields.io/badge/THARUSHI-COHNDSE242F--066-blueviolet?style=for-the-badge&logo=academia&logoColor=white" alt="THARUSHI"/></td>
  </tr>
</table>

<div align="center">
  
  ### **Group No: 13** | **Subject: Data Management 2**
  
  ![Team Badge](https://img.shields.io/badge/Team_UrbanFood-Group_13-success?style=for-the-badge&logo=github&logoColor=white)
  
</div>

## 🏫 Campus Information

<div align="center">
  <a href="https://www.nibm.lk" target="_blank">
    <img src="https://img.shields.io/badge/NIBM-National_Institute_of_Business_Management-003366?style=for-the-badge&logo=internet-explorer&logoColor=white" alt="NIBM">
  </a>
  
  ### School of Computing & Engineering
  
  <img src="https://img.shields.io/badge/Higher_National_Diploma-Software_Engineering-blue?style=for-the-badge&logo=graduation-cap&logoColor=white" alt="HND in SE">
  <img src="https://img.shields.io/badge/Batch-2024.2-blue?style=for-the-badge&logo=calendar&logoColor=white" alt="Batch 2024.2">
</div>

<details>
<summary>📚 About NIBM</summary>
<br>

The **National Institute of Business Management (NIBM)** is a premier educational institution in Sri Lanka offering a range of diploma and degree programs. The School of Computing & Engineering provides industry-focused education in various IT disciplines.

Visit [nibm.lk](https://www.nibm.lk) for more information.

</details>

## 📬 Contact Information


<table align="center">
  <tr>
    <th>Team Member</th>
    <th>Contact</th>
  </tr>
  <tr>
    <td>Bimsara</td>
    <td><a href="mailto:COHNDSE242F-047@student.nibm.lk"><img src="https://img.shields.io/badge/Email-COHNDSE242F--047-orange?style=flat-square&logo=gmail&logoColor=white" alt="Bimsara Email"></a></td>
  </tr>
  <tr>
    <td>Isura</td>
    <td><a href="mailto:COHNDSE242F-048@student.nibm.lk"><img src="https://img.shields.io/badge/Email-COHNDSE242F--048-orange?style=flat-square&logo=gmail&logoColor=white" alt="Isura Email"></a></td>
  </tr>
  <tr>
    <td>Ravindu</td>
    <td><a href="mailto:COHNDSE242F-049@student.nibm.lk"><img src="https://img.shields.io/badge/Email-COHNDSE242F--049-orange?style=flat-square&logo=gmail&logoColor=white" alt="Ravindu Email"></a></td>
  </tr>
  <tr>
    <td>Janindu</td>
    <td><a href="mailto:COHNDSE242F-064@student.nibm.lk"><img src="https://img.shields.io/badge/Email-COHNDSE242F--064-orange?style=flat-square&logo=gmail&logoColor=white" alt="Janindu Email"></a></td>
  </tr>
  <tr>
    <td>Jithmitha</td>
    <td><a href="mailto:COHNDSE242F-065@student.nibm.lk"><img src="https://img.shields.io/badge/Email-COHNDSE242F--065-orange?style=flat-square&logo=gmail&logoColor=white" alt="Jithmitha Email"></a></td>
  </tr>
  <tr>
    <td>Tharushi</td>
    <td><a href="mailto:COHNDSE242F-066@student.nibm.lk"><img src="https://img.shields.io/badge/Email-COHNDSE242F--066-orange?style=flat-square&logo=gmail&logoColor=white" alt="Tharushi Email"></a></td>
  </tr>
</table>

<div align="center">
  <a href="https://github.com/MrVinzSL">
    <img src="https://img.shields.io/badge/GitHub-MrVinzSL-black?style=for-the-badge&logo=github&logoColor=white" alt="Janindu Vinsura GitHub">
  </a>
</div>

## 🎬 Demo

<div align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExYWVrczJ3ZHJkbXhoNjl6N3kxZnB2bmJjbzBmYTlkaDgwOWl5ZjdyOCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/fvRAi1rD3zF0bxDCu0/giphy.gif">
  
  <h3>Watch our project demonstration video!</h3>
  
  <a href="https://drive.google.com/file/d/1KwjudGJRlvS6HgIo_CtYlgwf0VRFHw5W/view?usp=drive_link" target="_blank">
    <img src="https://img.shields.io/badge/⚡_Watch_Demo_Video_⚡-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Demo Video">
  </a>
</div>

## 📊 **Entity Relationship (ER) Diagram**  
Check out our **ER Diagram** for a detailed look at the core entities and relationships driving **UrbanFood**.

[![View ER Diagram](https://img.shields.io/badge/View%20ER%20Diagram-Link%20Here-blue)](https://drive.google.com/file/d/1ElDqNp5TALURasoqKArkJBq7NIRTfarV/view?usp=drive_link)

---

**Note:** The button above will take you directly to our ER Diagram hosted on Google Drive for easy viewing and understanding of the database structure.

---

<div align="center">
  
  <h3>⭐ Thank you for checking out our project! ⭐</h3>
  
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExODM3NGRkMjhhOGI0ZjVkMzI5Y2ZmYWVhMDFhYjliYmYyOWRhODUwNSZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/QTfX9Ejfra3ZmNxh6B/giphy.gif" width="300px" alt="Thank You">
  
  <p>© 2025 UrbanFood Team • All Rights Reserved</p>
  
</div>
