
1. select COUNT (*)
    from users


2. select count (*)
  from transfers 
where currency = 'CFA'


3. select distinct count (u_id)
   from transfers
where send_amount_currency = 'CFA'


4. select extract (month from when_created),sum(amount), count(atx_id)
from agent_transactions where extract (year from when_created)=2018
group by extract (month from when created;)


5.select (agent_id), sum(amount)
from agent_transactions
where when_created > now ()- interval '1 week'
group by agent_id
