# merchant-api

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
- ✨ response 

{
“id”:10001002,
   "name":"tajEldeen Hassan",
   "token":"access token"
}


```
# home screen Api 

```sh
- ✨ body
{
"date_from":"10/11/2022",
"date_to":"10/11/2022"
}

```

```sh
- ✨ response 
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

# Stock Api 
```sh
- ✨ body

sort by quantity,
search by name

```

```sh
- ✨ response 
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
- ✨ response 
sort by quantity,
sort by price,
```

```sh
✨ body
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
[https://dillinger.io][PlDb]
