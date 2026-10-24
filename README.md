Product.cs using System; 
using System.Collections.Generic;	 using System.Linq;	 using System.Web;	 
 
	namespace 	Product_Catalog	.Models 
{ 
	    public class Product	 
    {         public int Id { get; set; }	         public string Name { get; set; }	         public string Description { get; set; }	         public string Category { get; set; }	 
	        public int Price { get; set; }	 
 
 
 
Code: ProductController.cs using System.Collections.Generic; using System.Linq; using System.Web.Mvc; 
	using Product_Catalog.Models;	 
 
 
 
 
	            	Product product = GetProducts()	 
	                	.FirstOrDefault(p => p.Id == id.Value);	 
 
 
 
    
} 
  
Code:Index.cshtml 
 
	@model List<Product_Catalog.Models.Product>	 
 
 
 
	<h2>Product List</h2>	 
 
 
     
 
Code: Details.cshtml 
 
	@model Product_Catalog.Models.Product	 
 
 
 
	<h2>Product Details</h2>	 
 
 
            
                 
                                  
                 
            
</table>
 
	<br />	 
 
	@Html.ActionLink("Back to Product List", "Index")	 
 
 
  
<img width="468" height="535" alt="image" src="https://github.com/user-attachments/assets/9e83f504-b7a0-450c-92ef-7133935419df" />

