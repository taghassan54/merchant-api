# merchant-api

- [home screen Api](#home-screen-api)
- [login Api](#login-api)
- [Stock Api](#stock-api)
- [products Api](#products-api)
- [Transaction Api](#transaction)
- [Workers Api](#workers)
- [add Worker Api](#add-worker)
- [Orders Api](#orders)
- [images upload](#images-upload)
- [add stock](#add-stock)

# important note all data inside this dashboard belongs to current merchant branch or all branches if  that option selected

# login Api
```sh
- ✨ body
{
   "userName":"taghassan54",
   "password":"12345678",
   "rememperMe":true
}

```

```sh
 ✨ response 

{
“id”:10001002,
   "name":"tajEldeen Hassan",
   "token":"access token"
}


```
# home screen Api 

```sh
 ✨ body
{
"date_from":"10/11/2022",
"date_to":"10/11/2022"
}

```

```sh
 ✨ response 
{
"today_income":9500,
"this_week_income":560049,
"this_month_income":938472638,
"new_customer":10,
"pending_queue":220,
"complete_queue":9000,
"top_products":[
   {
       "id":1,
       "name":"product name",
       "sales":7000
   },
     {
       "id":2,
       "name":"product 2 name",
       "sales":8000
   }
],
 
"yearly_income":[
"2010":2030,
"2011":3948,
"2012":2987,
.... etc
],
 
"monthly_income"[
   "january":98266,
   "february":37563,
   "march":36528,
   "april":34678943,
   ... etc
],
 
"daily_income":[
   "saturday":4374,
   "sunday":3827,
   "monday":32863
   .... etc
],
 
}

```
# Add Stock 
```sh
 ✨ body
{
  "category":"1234",
  "productId":"34567",
  "manufacturingDate":""
  "expiryDate":"",
  "batchNo":"32456789",
  "price":"23456789",
  "quantity":"234567"
}

```

```sh
 ✨ response 
 
 ## 200
 {
    "status":"success",
    "message":"saved successfully !",
 } 
 
 ## 400
  {
    "status":"error",
    "message":"data error !",
 } 
```


# Stock Api 
```sh
 ✨ body

sort by quantity,
search by name

```

```sh
 ✨ response 
{
    "stock":[
        {
            "id":12908,
            "name":"products name",
            "category":"category name",
            "unitPrice":300,
            "quantity":800,
            "image":"image path"
        },
          {
            "id":12908,
            "name":"products name",
            "category":"category name",
            "unitPrice":300,
            "quantity":800,
            "image":"image path"
        },
          {
            "id":12908,
            "name":"products name",
            "category":"category name",
            "unitPrice":300,
            "quantity":800,
            "image":"image path"
        }
    ]
}

```
# products Api 

```sh
✨ body
sort by quantity,
sort by price,
```

```sh

- ✨ response 
{
    "categories":[
        {
            "id":2809,
            "name":"category name",
            "products":[
                {
                    "id":2738,
                    "name":"product Name",
                    "price":8368,
                    "quantity":926,
                     "image":"image path"
                },
                {
                    "id":2738,
                    "name":"product Name",
                    "price":8368,
                    "quantity":926,
                     "image":"image path"
                },
                {
                    "id":2738,
                    "name":"product Name",
                    "price":8368,
                    "quantity":926,
                     "image":"image path"
                },
                {
                    "id":2738,
                    "name":"product Name",
                    "price":8368,
                    "quantity":926,
                     "image":"image path"
                },
                {
                    "id":2738,
                    "name":"product Name",
                    "price":8368,
                    "quantity":926,
                     "image":"image path"
                }
            ]
        }
    ]
}

```

# Transaction

```sh
 ✨ body
{
"date_from":"10/11/2022",
"date_to":"10/11/2022",
"cashierId":10001002,
"productId":329,
"categoryID":56789,
}
```

```sh
✨ response 
[
    {
        "Ref No":"4535-dxb",
        "Username":"tajEldeen Hassan",
        "TransactionNo":"8864770",
        "Voucher":"22-148702",
        "Date":"29/11/2022",
        "Payment":"cash",
        "Total":"390.5",
        "Details":[
            {
                "ProductName":"Name",
                "Category":"Category",
                "SubCategory":"Sub - Category",
                "Quantity":"30",
                "Price":"4590",
                "Total":"2343545"
            }
        ]
    }
]

```
# add Worker

```sh
✨ body
{
"name":"tajEldeen Hassan",
"password":"1234",
"role":"role"
}
```

```sh
 ✨ response 
 
 ## 200
 {
    "status":"success",
    "message":"saved successfully !",
 } 
 
 ## 400
  {
    "status":"error",
    "message":"data error !",
 } 
```

# Workers

```sh
✨ body
{
"date_from":"10/11/2022",
"date_to":"10/11/2022",
// sorted by sales
}
```

```sh
 ✨ response 

[
    {
        "Name": "Name",
        "Sales": "3009",
        "image": ""
    },
        {
        "Name": "Name",
        "Sales": "3009",
        "image": ""
    },
        {
        "Name": "Name",
        "Sales": "3009",
        "image": ""
    },
        {
        "Name": "Name",
        "Sales": "3009",
        "image": ""
    }
]
```

# Orders

```sh 
✨ response 


[
    {
        "OrderID":"P8QMW6XHBDTS",
        "CreatedAt":"08/21/2019 12:34",
        "TimeSlot":"1:00 pm - 2:00pm",
        "Status":"Delivery",
        "Subtotal":"6523787",
        "DeliveryCharges":"7",
        "Payment Method":"visa",
        "Total":"6578239",
        "Products":[
             {
                "ProductName":"Name",
                "Category":"Category",
                "SubCategory":"Sub - Category",
                "Quantity":"30",
                "Price":"4590",
                "Total":"2343545"
            }
        ]
    }
]

```

 # images upload
```sh
// type may be = default_logo , main_logo ,footer_logo ,printing_logo
✨ body{
  "type":"default_logo",
  "file": file
}

```

```sh
 ✨ response 
 
 ## 200
 {
    "status":"success",
    "message":"saved successfully !",
 } 
 
 ## 400
  {
    "status":"error",
    "message":"data error !",
 } 
 ```

[edit](https://dillinger.io)
