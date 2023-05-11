# dotDigital

Here I saved some special code for a DotDigital (DotMailer). 

### Tips and Trick:
- DD shrink JPG to content width. This is a problem to use JPG for retina and other high resolution displays. To bypass this problem you can just change the .jpn -> .png in file name and upload it to DD. It will think this is a PNG and will not reduice this size
- Use upload image in template. Use this domain: "https://i.emlfiles.com/cmpimg/"


### Notes:
- It should take up to 1 hour to show up as webinsight data on Dotdigital, unfortunately, there isn't a way to push that data manually. 
- Support is not a technical. It's nice, but not too helpful, so you need to ask them to create a ticket for you and there you will can find Technical team.
- Programs contact enrolment. DotDigital allow up to around 20-30 mins in extreme cases. Basically, contact can start to pass nodes from 2-30 min. 



### Codes:

All liquid code need to be wrapped in "<!-- -->" as it will not work correctly.

#### Issue with Abandoned Browsering Special Price as null.
    <div>
      <!--{% if PageValues.product_specialprice > 0.00 %}-->
        <p class="productfield product-price_incl_tax" style="color: rgb(116, 121, 101);"><strike>{{ PageValues.product_price_incl_tax | money: 'ga-IE' }}</strike>               </p>
        <p class="productfield product-specialprice_incl_tax" style="color: rgb(6, 6, 6);"><b>{{ PageValues.product_specialprice_incl_tax | money: 'ga-IE' }}</b></p>
      <!--{% else %}-->
        <p style="color: rgb(6, 6, 6);" text-decoration:none;"><b>{{ PageValues.product_price_incl_tax | money: 'ga-IE' }}</b></p>
      <!--{% endif %}-->
    </div>
                                                         

    
