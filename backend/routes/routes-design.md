**Order Route**

- `POST {HOST}/order/new`: Requires authentication. Creates a new order.
- `GET {HOST}/order/:id`: Requires authentication. Retrieves information about a specific order identified by the order ID.
- `GET {HOST}/orders/me`: Requires authentication. Retrieves all orders associated with the authenticated user.
- `GET {HOST}/admin/orders`: Requires authentication. Requires "admin" role authorization. Retrieves all orders in the system. Only accessible to administrators.
- `PUT {HOST}/admin/order/:id`: Requires authentication. Requires "admin" role authorization. Used to update a specific order identified by the order ID. Only accessible to administrators.
- `DELETE {HOST}/admin/order/:id`: Requires authentication. Requires "admin" role authorization. Used to delete a specific order identified by the order ID. Only accessible to administrators.

**Product Route**

- `GET {HOST}/products`: Used to retrieve all products.
- `GET {HOST}/admin/products`: Requires authentication. Requires "admin" role authorization. Used to retrieve all products in the system. Only accessible to administrators.
- `POST {HOST}/admin/product/new`: Requires authentication. Requires "admin" role authorization. Used to create a new product. Only accessible to administrators.
- `PUT {HOST}/admin/product/:id`: Requires authentication. Requires "admin" role authorization. Used to update a specific product identified by the product ID. Only accessible to administrators.
- `DELETE {HOST}/admin/product/:id`: Requires authentication. Requires "admin" role authorization. Used to delete a specific product identified by the product ID. Only accessible to administrators.
- `GET {HOST}/product/:id`: Used to retrieve details of a specific product identified by the product ID.
- `PUT {HOST}/review`: Requires authentication. Used to create a review for a product.
- `GET {HOST}/reviews`: Used to retrieve all reviews for a product.
- `DELETE {HOST}/reviews`: Requires authentication. Used to delete a review. Requires authentication.

**User Route**

- `POST {HOST}/register`: Used to register a new user.
- `POST {HOST}/login`: Used to authenticate and log in a user.
- `POST {HOST}/password/forgot`: Used to initiate the password reset process by sending a reset password email to the user.
- `PUT {HOST}/password/reset/:token`: Used to reset the user's password using the reset token received via email.
- `GET {HOST}/logout`: Used to log out the currently authenticated user.
- `GET {HOST}/me`: Requires authentication. Used to retrieve the details of the authenticated user.
- `PUT {HOST}/password/update`: Requires authentication. Used to update the password of the authenticated user.
- `PUT {HOST}/me/update`: Requires authentication. Used to update the profile information of the authenticated user.
- `GET {HOST}/admin/users`: Requires authentication. Requires "admin" role authorization. Used to retrieve all users in the system. Only accessible to administrators.
- `GET {HOST}/admin/user/:id`: Requires authentication. Requires "admin" role authorization. Used to retrieve information about a specific user identified by the user ID. Only accessible to administrators.
- `PUT {HOST}/admin/user/:id`: Requires authentication. Requires "admin" role authorization. Used to update the role of a specific user identified by the user ID. Only accessible to administrators.
- `DELETE {HOST}/admin/user/:id`: Requires authentication. Requires "admin" role authorization. Used to delete a specific user identified by the user ID. Only accessible to administrators.
