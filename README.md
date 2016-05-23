# Snippets
Snippets for visual studio

Replace your VisualStudion Code Snippets by this repo


#### HTML Snippets 

Filter Panel 
Shortcut **filterpanel**
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