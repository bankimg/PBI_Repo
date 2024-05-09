Total Sales by Brand = 
    CALCULATE( 
        [Total Sales], 
        ALLEXCEPT('Category', 'Category'[Brand]) 
    )
