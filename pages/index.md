# Parameterized Pages with Images

```category
select
category,count(1) cnt

from orders
group by 1
```

Click on a link below in the table to go to a specific page

<DataTable data={category} link=category showLinkCol=true/>
