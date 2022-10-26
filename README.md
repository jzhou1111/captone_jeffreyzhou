# captone_jeffreyzhou

SELECT a.Subscriber_Customer, count(*)
FROM 2019_q2 a
JOIN 2019_q3 b ON b.Subscriber_Customer = a.Subscriber_Customer
JOIN 2019_q4 c ON c.member_casual = a.Subscriber_Customer
JOIN 2020_q1 d On d.Subscriber_Customer = a.Subscriber_Customer
GROUP BY a.Subscriber_Customer

