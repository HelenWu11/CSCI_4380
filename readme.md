   Recommended Fishing Rivers And Streams (River_data)
    https://data.ny.gov/Recreation/Recommended-Fishing-Rivers-And-Streams/jcxg-7gnm

    Accessible Outdoor Recreation Destinations
    https://data.ny.gov/Recreation/Accessible-Outdoor-Recreation-Destinations/pt2v-9a3h

    Liquor Authority Quarterly List of Active linceses

    https://data.ny.gov/Economic-Development/Liquor-Authority-Quarterly-List-of-Active-Licenses/hrvs-fxs2


    National Register of Historic Places
    https://data.ny.gov/Recreation/National-Register-of-Historic-Places/iisn-hnyv



for our load_data:
1. We need use the schema.sql to set up the table and schema(include in the python code)
2. Then it would load four files separately.



General interface:
    #just a infinite loop to continue

    menu:
        at first, we would ask the user to write the location
        
        then get into the manu:
            *1. recommand (randomly choose the closest places for user)
                #the following 4 would be choose the closest place which the user is most interested in 
            2. Historic
            3. Outdoor
            4. Liquor
            5. Rivers

            *6. __2 or 3 or 4 or 5 or 6__(#) 
                # "#" is the number k, we can choose the place in k distance
            *7. __2 or 3 or 4 or 5 or 6__(#th)
                # "#" is the number of k, we can choose the kth closest places

            8. we allow two or three location search like : 
                Historic Outdoor------> Example a 
                Liquor Rivers
                Outdoor Liquor

                first we would search the first closest destination for Example a is Historic Place and then we would use the place of historic place to search the closest outdoor places 
            
            *9. connect the outdoor and the fisihing, maybe we can search that if the outdoor can fish, when and where and what kind of fish can get. 
            
