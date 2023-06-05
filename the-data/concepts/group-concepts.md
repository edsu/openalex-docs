# Group concepts

You can group concepts with the `group_by` parameter:

* Get counts of concepts by [`level`](concept-object.md#level):\
  [https://api.openalex.org/concepts?group\_by=level](https://api.openalex.org/concepts?group\_by=level)

Or you can group using one the attributes below.

{% hint style="info" %}
It's best to [read about group by](../../the-api/get-groups-of-entities/) before trying these out. It will show you how results are formatted, the number of results returned, and how to sort results.
{% endhint %}

### `/concepts` group\_by \_\_ attributes

* [`ancestors.id`](concept-object.md#ancestors)
* [`cited_by_count`](concept-object.md#cited\_by\_count)
* [`has_wikidata`](../../the-api/filters/filter-concepts.md#has\_wikidata)
* [`level`](concept-object.md#level)
* [`summary_stats.2yr_mean_citedness`](concept-object.md#summary\_stats)
* [`summary_stats.h_index`](concept-object.md#summary\_stats)
* [`summary_stats.i10_index`](concept-object.md#summary\_stats)
* [`works_count`](concept-object.md#works\_count)