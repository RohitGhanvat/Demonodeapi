//page 1
>list of city
>>(Get) http://localhost:8100/location
>list of shop
>>(Get) http://localhost:8100/shop
>shop on the  basis of  city
>>(Get) http://localhost:8100/shop?stateId=1
list of special
>>(Get) http://localhost:8100/special

//page 2
>list of shop on basis of meal
>>(Get) http://localhost:8100/shop?mealId=1
>filter on basis of cuisine
>>(Get) http://localhost:8100/filter/1?cuisineId=2
>filter on basis of cost 
>>(Get) http://localhost:8100/filter/1?lcost=450&hcost=1200
> sort on basis of cost
>>(Get) http://localhost:8100/filter/1?lcost=150&hcost=1200&sort=1

//page 3
>details of the shop
>>(Get) http://localhost:8100/details/14
>Menu of the shop
>>(Get) http://localhost:8100/menu/9

//page 4
>Menu details (selected item )
>>(Post)  http://localhost:8100/menuItem
[1,3,6]
>place order 
>>(Post) http://localhost:8100/placeorder

{
    "name":"rohit",
    "email":"rohit@gmail.com",
    "address":Home 37",
    "phone":6789987989,
    "cost":450,
    "menuItem":[3,7,1]
}

//page 5
>list of order placed
>>(Get) http://localhost:8100/order
>list of order placed of particular user
>>(Get) http://localhost:8100/orders?email=
>update order status
>>(Put) localhost:8100/updateOrder/1

//extra
>delete order
>>(Delete) localhost:8100/deleteOrder
