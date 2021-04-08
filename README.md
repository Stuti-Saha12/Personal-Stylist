# Personal-Stylist 
## Personal-Stylist for E-Commerce Site:
The main aim of this project is to create a perfect match for the existing clothes in a person's wardrobe. It allows customers to take photos of pieces that already exist in their wardrobe and complementing clothes would be referred to them that would suit that given piece in their wardrobe according to the given style preferences. 

## Working:
- Using Django's built in user authentication, users can create accounts and access all the features of the software by logging in.
- For vision detection features, the code has been connected to Google’s image recognition capabilities .i.e., Google Vision API for image labelling and tagging of explicit content. Once a user registers himself, a product set is created which stores all the images uploaded by the user and also his style preference.
- After logging in, the user is presented to the dashboard which allows the user to add clothes, select style preference, generate outfit and view his clothes. In the “Add Clothes” section, the user is required to enter his username, category and image of the piece for which he wishes to develop complementing pieces followed by choosing a style preference that suits him the best under “Choose a Style” tab. The uploaded images are manipulated and saved using the PILLOW module(.i.e., Python Imaging Library) which helps to read a large number of image formats.
- Each of the style preferences has many outfits linked to it that helps develop outfits for the user through the “Possible Item” model. The google Vision API compares the uploaded image with the images in the database and selects the one with the maximum similarity score. This is then used to generate the outfit. 
- After having selected from the given style preference options, the user is directed to the “Your Outfit” page which shows the complementary pieces that would match the given piece. The user is given the option to dislike as well. Having done so, the outfit will be added to the “Bad Outfit” model so that they are not presented in future.  

