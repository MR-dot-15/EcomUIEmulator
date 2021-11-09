# EcomUIEmulator

## Brief intro
* ```mainUI.c```
  * Is supposed to function as the primary interface
  * Log-in
  * Display products
  * Search for a product (?)
  * Add to cart
  * Display cart
  * Proceed to buying
  * Status: <i>Unknown</i>
* ```delivery.c```
  * Is supposed to 
      * set an <i>address</i>
      * fix a <i>time slot</i>
      * check availability of delivery van/ delivery facility
  * Should proceed to billing
  * Status: <i>Working</i>
  * Modification needed, ref to ToDo
* ```billing.c```
  * Is supposed to produce a bill...
  * And append the purchase details to a purchase-history doc
  * Generates a receipt in txt format, and display on CLI as well
  * Should come back to ```mainUI.c``` after termination
  * Status: <i>Working</i>
## Comments
* All the txt files mentioned sit inside ```/accessories```
* ```time.txt``` (availability of delivery van in a particular slot) can be modified
* ```pin.txt```... self-explanatory
* Search option in ```billing.c``` is dropped
* ```fgets``` in ```billing.c``` is replaced by```scanf["%[^\n]s", *string]```
* In ```mainUI.c```, the attributes of the structure "product"- reorder, i remain unused
* ```cart.txt``` has a one-time purpose, should be overwritten before every purchase
* Max cart size = 10
* ```invoices.txt``` contain entire the purchase history
* ```Nov__9_2021.txt``` is a demo receipt
## ToDo
- [ ] ```mainUI.c```: addtocart() function should reduce # of available products
- [ ] ```mainUI.c```: a search() function, as it's asked for in the question
- [ ] ```mainUI.c```: <b>(IMPORTANT)</b> A user needs to log-in, using a unique ID. Probably this ID would be asociated to a few address options, aready stored (refer to the next point)
- [ ] ```delivery.c```: address should be set from a list (as the assignment suggests)
- [ ] ```delivery.c```: address to be passed to the billing stage
