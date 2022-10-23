# Functional Test Cases for Monobrand e-commerce [Levi's](https://www.levi.com/US/en_US/)

Prepared by **Matsvei Shydlouski**, student of the MMF (9-th group)

General preconditions:

- Shipping destination: USA
- Language: English

## Test Case №1 (Adding item to the bag)

### Preconditions: 

- [Product](https://www.levi.com/US/en_US/jeans-by-fit-number/men/jeans/511/511-slim-cut-off-10-11-mens-shorts/p/365550275) page is opened
- Valid size of the product is chosen (28 size)

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |                                                   
| 1 | Click on _Add to bag_ | Pop-up with added item appeared                                                 
| 2 | Click on _Bag_ | Page with a bag appeared and desired product has been added to the cart   

## Test Case №2 (Removing item from the bag)

### Preconditions: 

- [Bag](https://www.levi.com/US/en_US/cart) is opened
- [Product](https://www.levi.com/US/en_US/jeans-by-fit-number/men/jeans/511/511-slim-cut-off-10-11-mens-shorts/p/365550275) is added to the bag

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on _Remove_ | Bag page is re-rendered and item is removed (0 items)                                                     

## Test Case №3 (Adding item to favorites)

### Preconditions: 

- [Product](https://www.levi.com/US/en_US/clothing/men/outerwear/trucker-jacket/p/723340134) page is opened
- Size of the product is chosen (XS size)
- User is authorized to the app (Signed up/Loged in)

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on favorites button (heart) | Pop-up with added item appeared                                                     
| 2 | Click on _Favorites_ | Page with a favorites appeared and desired product has been added to the favorites                                                

## Test Case №4 (Removing item from the favorites)

### Preconditions: 

- [Product](https://www.levi.com/US/en_US/clothing/men/outerwear/trucker-jacket/p/723340134) page is opened
- [Product](https://www.levi.com/US/en_US/clothing/men/outerwear/trucker-jacket/p/723340134) is added to the favorites
- User is authorized to the app (Signed up/Loged in)

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on favorites button (heart) | Pop-up with message that item was removed from favorites appeared
| 2 | Click on _Favorites_ | Page with a favorites appeared and there are no items here (0 items)    

## Test Case №5 (Attempting to add item to the bag that is out of stock)

### Preconditions: 

- [Product](https://www.levi.com/US/en_US/clothing/men/outerwear/trucker-jacket/p/723340632) page is opened

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on invalid size (XS) | Page re-rendered and _Notify Me If in Stock_ button appeared                                                     

## Test Case №6 (Attempting to enter an incorrect email address to find out when the product will be in stock)

### Preconditions: 

- [Product](https://www.levi.com/US/en_US/clothing/men/outerwear/trucker-jacket/p/723340632) page is opened
- Invalid size of the product is chosen (XS size)

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on _Notify Me If in Stock_ button | Pop-up with form apperead                                             
| 2 | Type _abc.def@mail_ and click _Submit_ button | Nothing happened, site put error message (Please enter a valid email.)                                           

## Test Case №7 (Changing number of added products to bag)

### Preconditions: 

- [Bag](https://www.levi.com/US/en_US/cart) is opened
- [Product](https://www.levi.com/US/en_US/jeans-by-fit-number/men/jeans/511/511-slim-cut-off-10-11-mens-shorts/p/365550275) is added to the bag
- Valid size of the product is chosen (28 size)

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on select option and choose _6_ | Page is re-rendered and total has been recalculated (Before: $49.50 + $7.95 for shipping = $57.45, after: 6 * $49.50 + $0.00 for shipping = $297.00)                                                  

## Test Case №8 (Sorting clothes by _Price Low-High_)

### Preconditions: 

- [Kids category page](https://www.levi.com/US/en_US/clothing/kids/c/levi_clothing_kids) is opened

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on _Sort By_ button and choose _Price Low-High_ | Page is re-rendered and now there are clothes with the lowest price of the chosen category (starting with $6.98)            

## Test Case №9 (Filtering clothes by price)

### Preconditions: 

- [Kids category page](https://www.levi.com/US/en_US/clothing/kids/c/levi_clothing_kids) is opened

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Find _Price_ filter and choose _$75-$100(3)_ | Page re-rendered and there are 3 clothes on the page with the price $76.00, $78.00 and $78.00                     

## Test Case №10 (Attempting to type an incorrect promo code)

### Preconditions: 

- [Bag](https://www.levi.com/US/en_US/cart) is opened

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Type _ILOVEMMF_ and press enter | Nothing happened, site put error message (ILOVEMMF is not valid. Check your entry and try again.)                               
