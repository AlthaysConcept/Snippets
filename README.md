# Snippets
Snippets for visual studio

Replace your VisualStudion Code Snippets by this repo


#### HTML Snippets 

**Filter Panel**
shortcut :  **filterpanel**
```html

<div id="filter-group" class="panel-group">
    <div class="panel panel-filter">
        <div class="panel-heading"  data-toggle="collapse" href="#purchase-request-index-search-collapse">
            <h4 class="panel-title">
                @Html.Raw(ApplicationString.SEARCHFILTER)
            </h4>
        </div>
        <div id="purchase-request-index-search-collapse" class="panel-collapse collapse">
            <div class="panel-body">
            <!-- PASTE FORMS HERE -->
            </div> 
        </div>
    </div>
</div>

```

#### CSharp Snippets

** ProcessApiResponse ** shortcut : **PAR**
```C#

ProcessAPIResponse(response,
                    ref result,
                    () => {/* OK */ },
                    () => { /* Final */ return null; },
                    () => { /* Unauthorized */ },
                    () => { /* Error */ },
                    () => { /* BadRequest */ }

```

** SQLHelper ** shortcut : **sqlh**
```C#

SQLHelper sqlh = new SQLHelper("ConnectionString");
SQLResponse sqlr;

```

** SQL Select fields ** shortcut : **sf**
```C#

sqlh.Fields.Add("FIELDS");
sqlh.Table = "TABLE";
sqlh.Where = "param=@param";
sqlh.Parameters.Add(new SqlParameter("param", "value"));
sqlr = sqlh.ExecuteQuery();
if (sqlr.Success && sqlr.Results.Count > 0)
{
    var data = sqlr.Results[0][0];
}
sqlh.Clear();

```

** Select Fields (execRowQuery) ** shortcut : **erq**
```C#

string query = "QUERY";
sqlh.Parameters.Add(new SqlParameter("param", "value"));
SQLResponse sqlr = sqlh.ExecuteRawQuery(query, QueryType.);
if (sqlr.Success && sqlr.Results.Count > 0)
{
    var data = sqlr.Results[0][0];
}
sqlh.Clear();

```