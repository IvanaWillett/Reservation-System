# SmartQ Reservation System

This web application is the term project for the CPS 731 Software Engineering I course at Toronto Metropolitan University for the Fall 2024 semester.

The aim of the web application is to provide a unified interface for restaurant staff to view and manage reservations and track the availability of tables, and for customers to make reservations at their favorite restaurants in as easy a manner as possible.

The web app makes extensive use of Supabase's realtime features to subscribe to database changes for scenarios where a reservation is made, for example. A simple in-app notification system was also created to take advantage of the realtime features. This notification system allows a restaurant to send notifications to their reservees and keep them updated.

A drag-and-drop floor plan creator was also implemented which allows managers to intuitively create custom floor plans for restaurants.

Created with: 
- **React**
- **Supabase + PostgreSQL**
- **TailwindCSS + Shadcn/ui**
  
Tested with: 
- **Vitest**
- **React Testing Library**
- **System test cases** derived from the project use case model.

Hosted on:
- Render

Live deployment
---
https://smartq.onrender.com

###### *It might take a while for the app to load on first visit. The app is hosted on Render's hobby plan, which spins down the app after a period of inactivity. The slow load isn't caused by a lack of performance in the app itself.

To appreciate the realtime functionalities of the web app, consider running the app on two separate browsers, side by side. Log in with a customer account on one instance and either an employee or a manager account on the other instance, then test the app. 

###### *Manager accounts have access to more features than employee accounts.

Local Deployment
---
Before running the application for the first time, please ensure that the neccessary files are installed.


Installation of necessary files: 
```
npm install 
```

To run the application, cd into the reservation-system directory and run the following command: 
```
npm run dev
```

###### *The commands above only work if you have been given the .env file.

Project Demo
---
https://youtu.be/skylZBg40po

Screenshots
---

1. Landing Page <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 29 41 PM" src="https://github.com/user-attachments/assets/2a80d1c7-8dfd-4e83-a405-029fcc12253a" />
2. Create Account <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 33 42 PM" src="https://github.com/user-attachments/assets/7d9b0c24-97a8-4063-9d5d-060f39db5443" />

3. Login <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 34 53 PM" src="https://github.com/user-attachments/assets/66a76f84-2ef0-4b65-b7a1-9707b26ec0ec" />

4. Customer Dashboard <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 30 16 PM" src="https://github.com/user-attachments/assets/a0cae6ca-71a3-4d4a-b2ad-1069102df182" />

5. Customer Reservation <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 30 25 PM" src="https://github.com/user-attachments/assets/d7f767bc-907b-48c4-945d-4c275c3f79bb" />

6. Staff Dashboard <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 29 26 PM" src="https://github.com/user-attachments/assets/1a3f6086-7989-4e8b-9ac3-4fc26db10a52" />

7. Manage Floorplans <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 29 07 PM" src="https://github.com/user-attachments/assets/c4772201-2c37-40e6-bb21-05f7a094dc00" />

8. Create Floorplan <img width="1920" height="993" alt="Screenshot 2025-07-23 at 3 28 55 PM" src="https://github.com/user-attachments/assets/7589fee0-57c1-4f2d-9337-c62c7abdaf77" />

Fake credentials for testing
---
The following credentials were arbitrarily created and some were used to manually test the application. 


You may use any of them or create your own fake credentials to try out the app.

```javascript
[
  {  //account created; use for login; customer
    "firstName": "Sarah",
    "lastName": "Mitchell",
    "email": "sarah.mitchell@example.com",
    "phone": "555-123-4567",
    "password": "Kj#9mP2$"
  },
  {  //account created; use for login; manager
    "firstName": "Marcus",
    "lastName": "Rodriguez",
    "email": "m.rodriguez@example.com",
    "phone": "555-987-6543",
    "password": "Nh5$pL8@"
  },
  {  //account created; use for login; employee
    "firstName": "Emily",
    "lastName": "Thompson",
    "email": "emily.t@example.com",
    "phone": "555-456-7890",
    "password": "Wx7&nD9#"
  },
  {
    "firstName": "James",
    "lastName": "Wilson",
    "email": "jwilson@example.com",
    "phone": "555-234-5678",
    "password": "Qb4$mH9!"
  },
  {  //account created; use for login; manager
    "firstName": "Lisa",
    "lastName": "Chen",
    "email": "l.chen@example.com",
    "phone": "555-345-6789",
    "password": "Yd5@jR7*"
  },
  {  //account created; use for login; customer
    "firstName": "Elena",
    "lastName": "Kovacs",
    "email": "elena.kovacs@example.com",
    "phone": "555-678-9012",
    "password": "Rt6#qM3!"
  },
  {
    "firstName": "David",
    "lastName": "Nguyen",
    "email": "d.nguyen@example.com",
    "phone": "555-890-1234",
    "password": "Zx9$fK4@"
  },
  {  //account created; use for login; customer
    "firstName": "Olivia",
    "lastName": "Patel",
    "email": "olivia.patel@example.com",
    "phone": "555-567-8901",
    "password": "Jh7*nL2#"
  },
  {
    "firstName": "Michael",
    "lastName": "Garcia",
    "email": "m.garcia@example.com",
    "phone": "555-345-6789",
    "password": "Bq5%tP8$"
  },
  {
    "firstName": "Rachel",
    "lastName": "Kim",
    "email": "rachel.kim@example.com",
    "phone": "555-234-5678",
    "password": "Ck3@wS6!"
  },
  {
      "firstName": "Alexander",
      "lastName": "Singh",
      "email": "a.singh@example.com",
      "phone": "555-456-7890",
      "password": "Gm9#nK4$"
    },
    {
      "firstName": "Isabella",
      "lastName": "Martinez",
      "email": "isabella.m@example.com",
      "phone": "555-567-8901",
      "password": "Wq7*fL2!"
    },
    {
      "firstName": "Jordan",
      "lastName": "Brown",
      "email": "jordan.brown@example.com",
      "phone": "555-678-9012",
      "password": "Hy5@pT3#"
    },
    {
      "firstName": "Sophie",
      "lastName": "Lee",
      "email": "sophie.lee@example.com",
      "phone": "555-789-0123",
      "password": "Jx6$nR9@"
    },
    {
      "firstName": "Daniel",
      "lastName": "Miller",
      "email": "d.miller@example.com",
      "phone": "555-890-1234",
      "password": "Bk4!mQ7%"
    }
]

```
