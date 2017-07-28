# How-to-store-id-through-select-option
&lt;select name="product_cat">  &lt;option value="&lt;?php echo $cat_id; ?>">&lt;?php echo $cat_title; ?>&lt;/option>  &lt;?php   $qry=mysqli_query($db,"select * from categories");   while($row_cat=mysqli_fetch_array($qry))   {    extract($row_cat);    echo "&lt;option value='$cat_id'>$cat_title&lt;/option>";   }   ?>  &lt;/select>
