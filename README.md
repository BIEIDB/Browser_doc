# Pre requirements:
* You've got Kibana 6.5.4 installed and connected to the ElasticSearch version 6.5 or higher.
* You've got terminal access to install plugin.

### Indexes specification

On version 0.1.x we doen't support nested types. You can see all nested object with our "Show JSON" feature.
We'll add nested types browsing support in our future versions, stay tuned.

Arrays are displayed in one row.

You can get list of unique terms only for *keyword* and integer types.
You can also get unique terms for text fields if it has *keyword* type in it's multitype mapping. 

Sorting ability works for simple types works almost like in the ElasticSearch.
For *text* type fields it's recommended to have *keyword* multitype set.

## Installation

To run installation you should run in the terminal on your Kibana server:

    bin/kibana-plugin install file:///some/local/path/biei-0.1.zip


If you have any questions about installation process, please check the Kibana manual [page](https://www.elastic.co/guide/en/kibana/current/install-plugin.html) or contact us at [support@bieidb.com](mailto:support@bieidb.com).

## Configuration
Your BIEI browser is up and running. Now it's time to configure it.
Visit [http://kibana-server/app/bieibro](http://kibana-server/app/bieibro)
Firstly, you need to add indexes you're interested in.

* Click on the gear wheel icon in the up right corner of the browser window
 ![gear](/images/settings.png)

* You're on the configuration page. Now click on the plus icon on left panel
 ![plus](/images/add_node.png)

* Fill in fields in the appeared form. Select Index  node type, write a name and select one of the indexes from the list. Don't forget to select doc type as well.
 ![form](/images/add_node_form.png)
 
* Click on the Save button and new index node appears in the navigation tree.
* Now it's time to configure it's view.
* Click on the index node, you've already added. And select *Data settings*.
* Now you can configure columns visibility, order, width and labels.
 ![settings](/images/view_settings.png)
* You can also add logical node. In our browser they act as folders to organise your indexes. You can add folders to folders or indexes with drag and drop.
* Well done, you can go back to the main page and enjoy browsing of data indexes you've added Click on the home icon.
* Type something in the search input or browse your data by clicking on the indexes in the navigation tree.

## Using
With our browser you can save your favourite search requests by clicking on the star icon in the search input
 ![search](/images/search.png)
    

Use all power of our cool filters to narrow your searches.
 ![filters](/images/filters.png)
    

To make time-based filters work correctly, you need to choose field with the time type.
 ![time](/images/time_check.png)
    

You can always get unique values of field and get pure JSON of the string you're looking at.
    
And you can always add a value in the cell to the search string in 2 mouse click.
 ![menu](/images/menu.png)