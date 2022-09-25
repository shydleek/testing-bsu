# Test Cases for Monobrand e-commerce [Levi's](https://www.levi.com/US/en_US/)

Prepared by **Matsvei Shydlouski**, student of the MMF (9-th group)

## Test Case №1 (Sign up the app)

### Preconditions: 

- Website https://www.levi.com/US/en_US/ is opened

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on burger menu (=) | Burger menu appeared                                                     
| 2 | Click on _Sign Up_ | Pop-up with registration appeared                                                 
| 3 | Type _First Name_, _Second Name_ and try click to _Join_ | Nothing happened, site put error messages (Please enter a valid email. Passwords must be at least 8 characters. Please add more characters.)                         
| 4 | Type _Email_, _Password_ and try click to _Join_ | User authorized 

## Test Case №2 (Add Man Jacket to favourites)

### Preconditions: 

- Website https://www.levi.com/US/en_US/ is opened
- User is authorized to the app (Signed up/Loged in)

### Steps:

| №  | Action | Expected result                                                                 
| - | - | - |
| 1 | Click on burger menu (=) | Burger menu appeared                                                     
| 2 | Click on _MEN_ | New list of men items appeared                                                 
| 3 | Click on _Jean Jackets & Outerwear_ | Page of _MEN'S DENIM JACKETS & OUTERWEAR_ opened                            
| 4 | Choose a _Trucker Jacket_ | Page with a _Trucker Jacket_ opened
| 5 | Choose a _Rinse - Dark Wash_ color | Page rendered to the jacket with a chosen color
| 6 | Choose a _M_ size | _Favorite_ button is active now 
| 7 | Click on _Favorite_ button | Pop-up with added item to the favorites appeared 