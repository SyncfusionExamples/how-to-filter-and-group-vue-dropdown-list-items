<template>
    <div>
      <!-- <div id= "dropdownlist" style="margin:10% 40%; width:250px;">
        <br>
        <ejs-dropdownlist popupHeight="200px" popupWidth="250px" 
        :dataSource='dataItem' :fields='dataFields' 
        placeholder='Select a Name' :allowFiltering='true'
        :filtering='onFiltering'>
        </ejs-dropdownlist>
      </div> -->
      <div id= "dropdownlist" style="margin:10% 40%; width:250px;">
        <br>
        <ejs-dropdownlist popupHeight="200px" popupWidth="250px" 
        :dataSource='dataItem' placeholder='Select a Name'
        :allowFiltering='true' ignoreAccent='true'>
        </ejs-dropdownlist>
      </div>
    </div>
</template>

<script>
import Vue from "vue";
import { DropDownListPlugin } from "@syncfusion/ej2-vue-dropdowns";
Vue.use(DropDownListPlugin);
//import {Query} from "@syncfusion/ej2-data";
export default Vue.extend({
  data: function() {
    return {
       dataItem : [
            'Aeróbics',
            'Aeróbics en Agua',
            'Aerografía',
            'Aeromodelaje',
            'Águilas',
            'Ajedrez',
            'Ala Delta',
            'Álbumes de Música',
            'Alusivos',
            'Análisis de Escritura a Mano'
        ],
      // dataItem: [
      //   { Name: 'Cabbage', Category: 'Leafy and Salad', Id: 'item1' },
      //   { Name: 'Spinach', Category: 'Leafy and Salad', Id: 'item2' },
      //   { Name: 'Wheat grass', Category: 'Leafy and Salad', Id: 'item3' },
      //   { Name: 'Yarrow', Category: 'Leafy and Salad', Id: 'item4' },
      //   { Name: 'Pumpkins', Category: 'Leafy and Salad', Id: 'item5' },
      //   { Name: 'Chickpea', Category: 'Beans', Id: 'item6' },
      //   { Name: 'Green bean', Category: 'Beans', Id: 'item7' },
      //   { Name: 'Horse gram', Category: 'Beans', Id: 'item8' }
      //   ],
      // dataFields: { 
      //   groupBy: 'Category', 
      //   text: 'Name', 
      //   value: 'Id' }
    }
  },
    // methods: {
    //     onFiltering: function(e) {
    //         var filterQuery = new Query();
    //         //frame the query based on search string with filter type.
    //         filterQuery = (e.text !== '') ? filterQuery.where('Name', 'contains', e.text, true) : filterQuery;
    //         //pass the filter data source, filter query to updateData method.
    //         e.updateData(this.dataItem, filterQuery);
    //     }
    // }
});

</script>
<style>
@import url(https://cdn.syncfusion.com/ej2/material.css);
</style>