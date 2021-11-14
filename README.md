# EcomUIEmulator

## Brief intro
* ```mainUI.c```
  * Is supposed to function as the primary interface
  * Log-in
  * Display products
  * Search for a product
  * Add to cart
  * Display cart
  * Proceed to buying
  * Not maintained
* ```delivery_and_billing.c```
  * Redirected from ```mainUI.c```
  * Actions:
    * Checks the pin provided by the user against a precompiled list
    * If delivery is feasible, the user is asked for an address and their prefered delivery-timing
    * Proceeds to the billing section
      * Asks for the user's name
      * Generates an Invoice (outputted on terminal + saved as a txt)
      * Appends the recent purchase to a txt containing all their past purchases
      * <i>Should</i> redirect to the main UI
## Comments
* All the txt files mentioned sit inside ```/accessories```
* ```time.txt``` (availability of delivery van in a particular slot) can be modified
* ```pin.txt```... self-explanatory
* Search option in ```billing.c``` is dropped
* ```cart.csv``` has a one-time purpose, should be overwritten before every purchase
* Max cart size = 10
* ```invoices.txt``` contain entire the purchase history
* ```Nov_13_2021.txt``` is a demo receipt
## ToDo
All resolved :)
