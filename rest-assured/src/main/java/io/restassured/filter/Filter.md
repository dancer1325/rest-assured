* Check [documentation](https://github.com/dancer1325/rest-assured-wiki/blob/master/Usage.md#filters)
* if you need an ordered filter -> use `OrderedFilter`
* `Response filter()`
  * allows
    * filtering the
      * incoming request
      * response specifications
      * outgoing response
  * once ALL is done & you want to deliver the request -> call `FilterContext#next(FilterableRequestSpecification, FilterableResponseSpecification)`
  * if you want to abort the filter chain execution -> return a `Response` directly