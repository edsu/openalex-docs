# Sort entity lists

Use the `?sort` parameter to specify the property you want your list sorted by. You can sort by these properties, where they exist:

* `display_name`
* `cited_by_count`
* `works_count`
* `publication_date`
* `relevance_score` (only exists if there's a [search filter](sort-entity-lists.md#search) active)

By default, sort direction is ascending. You can reverse this by appending `:desc` to the sort key like `works_count:desc`. You can sort by multiple properties by providing multiple sort keys, separated by commas. Examples:

* All works, sorted by `cited_by_count` (highest counts first)\
  [https://api.openalex.org/works?sort=cited\_by\_count:desc](https://api.openalex.org/works?sort=cited\_by\_count:desc)
* All venues, in alphabetical order by title:\
  [https://api.openalex.org/venues?sort=display\_name](https://api.openalex.org/venues?sort=display\_name)

You can sort by relevance\_score when searching:

* Sort by year, then by relevance\_score when searching for "bioplastics"\
  [https://api.openalex.org/works?filter=display\_name.search:bioplastics\&sort=publication\_year:desc,relevance\_score:desc](https://api.openalex.org/works?filter=display\_name.search:bioplastics\&sort=publication\_year:desc,relevance\_score:desc)

An error is thrown if attempting to sort by relevane\_score without a search query.