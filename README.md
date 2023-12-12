# LittleLemon API: Advanced Features

Welcome to the Django LittleLemon API, an advanced and fully functional project tailored for the Little Lemon restaurant. This API empowers client application developers to create dynamic web and mobile applications. The system supports various roles, allowing users to interact with menu items, place orders, manage deliveries, and more.

## Features:

### Admin Capabilities:
- Assign users to the manager group.
- Access the manager group with an admin token.
- Add menu items.
- Add categories.

### Manager Capabilities:
- Log in.
- Update the item of the day.
- Assign users to the delivery crew.
- Assign orders to the delivery crew.

### Delivery Crew Capabilities:
- Access orders assigned to them.
- Update an order as delivered.

### Customer Capabilities:
- Register.
- Log in and obtain access tokens.
- Browse all categories.
- Browse all menu items.
- Browse menu items by category.
- Paginate menu items.
- Sort menu items by price.
- Add items to the cart.
- Access previously added items in the cart.
- Place orders.
- Browse their own orders.

## API Endpoints:

### User Registration and Token Generation:
- `/api/users`
- `/api/users/users/me/`
- `/token/login/`

### Menu Item Endpoints:
- `/api/menu-items`
- `/api/menu-items/{menuItem}` (repeat)
- `/api/menu-items` (repeat)

### User Group Management Endpoints:

#### Manager Group:
- `/api/groups/manager/users`
- `/api/groups/manager/users/{userId}`

#### Delivery Crew Group:
- `/api/groups/delivery-crew/users`
- `/api/groups/delivery-crew/users/{userId}`

### Cart Management Endpoints:
- `/api/cart/menu-items`

### Order Management Endpoints:
- `/api/orders`
- `/api/orders/{orderId}` (repeat)
