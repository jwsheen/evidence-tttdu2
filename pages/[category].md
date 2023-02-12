{$page.params.category}

```category
select
category,
'incredibles_5.svg' as logo_url, count(1) cnt

from orders
group by 1
```

## Markdown wont accept the js filter

![Logo]({category.filter(d => d.category === $page.params.category)[0].logo_url})

## But HTML will

### #1 filter category

<img src="{category.filter(d => d.category === $page.params.category)[0].logo_url}" alt=logo>

### #2 filter cnt

<img src="{category.filter(d => d.cnt === 611)[0].logo_url}" alt=logo>
