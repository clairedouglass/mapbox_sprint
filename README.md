# mapbox_sprint

Evaluating Performance of the Directions API for the month of May

Question:
How can we better understand new users of the "Directions" services?

2,069 users made directions API calls in May  
{code} SELECT count(distinct user_id) FROM mapbox.consumed_api_calls 
WHERE received_at >= '2017-05-01'
AND directions > 0 {code}

592 users made only directions API calls in May

{code} SELECT count(distinct user_id) FROM mapbox.consumed_api_calls 
WHERE received_at >= '2017-05-01'
AND directions > 0
AND geocode = 0
AND mapviews = 0 {code}

How many newly active users are using the directions API? 

Are they using this API in conjunction with other services?

How do people who signed up this month compare to prior months?

