# zoho_flight
Zoho Simple Flight ticket booking system

## Problem Statement

A airline operates multiple flights from Chennai to Mangalore. To write a basic
ticket booking program for their flights.

Usage

Booking

```
WELCOME TO ZOHO AIRLINES CHENNAI TO MANGALORE

Please enter your choice:(1 for booking,2 for cancellation): 1
Enter flight number:(a101 or a102) a101
Enter class:(e-Economy or b-Business) e
Enter number of bookings: 1
Do you want a meals for this booking?(y/n)y



Your booking id is:  3UWC
Enter number of seats: 2

Seat No:  1
Enter seat location:(row in number column in alphabet) 1_a
1_a
Your column look like: ['W', 'M', 'A', 'A', 'M', 'M', 'A', 'A', 'M', 'M', 'W']
W
Price for this seat is:  1200
1_a  meal ordered

Seat No:  2
Enter seat location:(row in number column in alphabet) 2_d
2_d
Your column look like: ['W', 'M', 'A', 'A', 'M', 'M', 'A', 'A', 'M', 'M', 'W']
A
Price for this seat is:  1200
2_d  meal ordered
Meal cost for this booking is INR:  400
{'3UWC': {'Flight_no': 'a101', 'class_type': 'e', 'Seat_prices': {'1_a': 1200, '2_d': 1200}, 'meal': 'y', 'meal_cost': 400}}
```

Cancellation

```
WELCOME TO ZOHO AIRLINES CHENNAI TO MANGALORE

Please enter your choice:(1 for booking,2 for cancellation): 2
Booking_ID(s) ['CSZB']
Already booked Seat(s) [['1_c']]
Enter booking id in which a seat is to be cancelled from the above ids: CSZB
['1_c']
Enter index of seat number to be cancelled from the above list: 1_c
{'CSZB': {'Flight_no': 'a101', 'class_type': 'e', 'Seat_prices': {'1_c': 1200}, 'meal': 'y', 'meal_cost': 200}}
{'CSZB': {'Flight_no': 'a101', 'class_type': 'e', 'Seat_prices': {}, 'meal': 'y', 'meal_cost': 200}}
```

