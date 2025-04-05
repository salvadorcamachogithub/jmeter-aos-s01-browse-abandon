Updated: 04.2025  
Script created by Salvador Camacho

This is a JMeter script, it can be used as is for Professional Performance Engineering (LRP)

For using it with Enterprise Performance Engineering (LRE) or Core Performance Engineering (LRC), zip the folder AOS-JMeter-S01 Browse Abandon

This script does the same steps and logic as the Web - HTTP/HTML script AOS-Web-S01 Browse Abandon

This script was created with best practices, so it is more resilient, such as:
* Transaction naming
* No add cookies
* No third party
* One validation per transaction
* Think times at the end of each transaction to better simulate user behavior
* Main URL parametrized, Public AOS by default

This script randomly selects a product from the category and then goes to it in transaction number 3 and adds it to the cart to then abandon the cart  
The Add To Cart step is "simulated" (it hits a random AOS product image) as there is no http traffic in AOS when adding to the cart

Think times were set random from 7.5 seconds to 15 seconds

This script has 5 transactions:  
AOS-JMeter-S01-01 Access AOS URL  
AOS-JMeter-S01-02 Go To Speakers  
AOS-JMeter-S01-03 Random Product  
AOS-JMeter-S01-04 Add To Cart  
AOS-JMeter-S01-05 Checkout