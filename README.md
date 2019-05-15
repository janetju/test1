select
  count(case_id)
from remedy_tickets
where
  assigned_to_group = 'HROA-Reporting Support'
  and date_trunc('month', create_date) = '2017-06-01'
