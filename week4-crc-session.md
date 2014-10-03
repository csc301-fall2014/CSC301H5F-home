# CRC Cards


 * Train
   * R
     * Has an identifier.
     * Knows its carts.
     * Knows its physical location (I owe you an argument for this shouldn't be the responsibility of this class)
   * C
     * Cart
 
 
 * Cart
   * R
     * Knows its seats, and their layout.
     * Physical Services
     * Knows which seats are taken.
 



 * TrainCompany
   * R
     * Knows its name, and routes
     * Can access routes given from and/or to station(s).
     * Can update the price of a route.
     * Can delete a route.
   * C
     * DirectRoute


 * DirectRoute
   * R
     * Train copmany
     * Train
     * From and to station
     * Departure/Arrival time.
     * Price.
   * C
     * TrainCompany
     * Train





As a train company manager, I want to specify arrival/departure times.
* Create a DirectRoute with an arrival and departure time.

As a train company manager, I want to list services that are available in each cart.
 * From a DirectRoute, we can get the Train.
 * From the Train, we can get all the Carts.
 * Each Cart knows its physical services.


As a train company manager, I want to specify which seats are available in each cart of a scheduled trip.
* From a DirectRoute, we can get the Train.
* From the Train, we can get all the Carts.
* Each Cart knows which seats are taken.


As a train company manager, I want to offer different prices during different times.
 * Specify the price of a DirectRoute.
 
As a train company manager, I want to offer different prices for different carts.
 * We're a little stuck, but we can make things better by defining the following interface
   * PriceCalculator, Interface
     * R
        * Copmute the price of an avialable seat
        * Knows the direct route it's associated with.
     * C
        * DirectRoute
        * Train
        * Cart
