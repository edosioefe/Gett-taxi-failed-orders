# Gett-taxi-failed-orders
Gett, previously known as GetTaxi, is an Israeli-developed technology platform solely focused on corporate Ground Transportation Management (GTM). They have an application where clients can order taxis, and drivers can accept their rides (offers). At the moment, when the client clicks the Order button in the application, the matching system searches for the most relevant drivers and offers them the order. In this task, we would like to investigate some matching metrics for orders that did not completed successfully, i.e., the customer didn't end up getting a car.

I'll be completing the following tasks from the dataset:
1.Build up distribution of orders according to reasons for failure: cancellations before and after driver assignment
2.Plot the distribution of failed orders by hours
3.Plot the average time to cancellation with and without driver, by the hour
4.Plot the distribution of average ETA by hours
5.Display failed orders on a map

Data variables:
order_datetime - time of the order

origin_longitude - longitude of the order

origin_latitude - latitude of the order

m_order_eta - time before order arrival

order_gk - order number

order_status_key - status, an enumeration consisting of the following mapping: 4 - cancelled by client, 9 - cancelled by system, i.e., a reject

is_driver_assigned_key - whether a driver has been assigned

cancellation_time_in_seconds - how many seconds passed before cancellation


---FINDINGS:
Most failed order are coming from reading city centre; especially near the train station

Huge amount of failed oreder are coming from the early hours of the morning (Between 7am-9am); most caancelations from this period
are due to a driver not being assigned(customers in a rush in the morning with going to work/education)
Average ETA during this period is also very high; likely due to busy time/rush hour.
Clear solution is to have more driver working during this period, can offer drivers higher pay rate for incentive.

Average cancellation time is higher when driver is assigned; customers are willing to wait longer for taxi to come as long as a driver is assigned




