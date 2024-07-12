# Project Plan

Pod Members: **Elizabeth, Maria and Evelyn**

## Problem Statement and Description


Consumers find it difficult to discover skincare products tailored to their unique skin needs, leading to unnecessary expenses and trial-and-error with various brands. 

The main purpose of this website is to create a comprehensive and personalized skincare platform that helps users identify effective skincare products tailored to their unique skin types and concerns. The platform aims to reduce the trial-and-error process and prevent unnecessary skin damage by providing personalized recommendations. Dreamskin simplifies the process of finding the perfect skincare products for each user, ensuring effective results and enhancing user experience.

## User Roles and Personas

User Roles: registered and non-registered users.

User personas: 
1. Carla is a 22 year old college student living in Florida. She has struggled with oily skin and acne since her teenage years, which made her passionate for skincare. She is an extrovert who loves to share her skincare journey and discoveries with her friends and followers on social media. She frequently follows beauty influencers for the latest trends and product recommendations. Her primary goals are to find effective products for oil control and acne management. Her website interaction would be four times a month.

2. Brandon is a 28 year old software engineer living in San Francisco. Married and family-oriented, he juggles his busy work schedule with spending quality time with his spouse. Brandon has dry skin and is particularly concerned about dark spots and achieving an even skin tone. He is organized and health-conscious, often researching the best skincare products to address his concerns. Due to his busy lifestyle, he typically accesses the skincare website about once a month, looking for effective and time-efficient solutions. His website interaction will be once a month. 

## User Stories

 **As a [user role], I want to [what], so that [why]**

1. As a user, I want acne prone skin products so I can stop breaking out.
2. As a user, I want personalized product recommendations so that I don't need to experiment with products.
3. As a user with sensitive skin, I want products without certain ingredients so that I dont cause further damage to my skin.
4. As a user, I want to learn more about skincare products so that I can make informed decisions.
5. As a busy individual, I want a simplified routine so that I can save time.
6. As a new user, I want to take a skincare quiz so that I can get personalized routine
7. As a new user, I want to receive personalized  skincare recommendations based on my skin concerns so that I can address my specific needs.
8. As a user, I want personalized sunscreen recommendations suitable for daily use to protect my skin from sun damage.
9. As a user, I want clear instructions on how to use recommended products to maximize benefits and ensure they are suitable for my skin type and concerns. 
10. As a user, I want a diverse range of skincare products available across different price points so that I can choose options that fit my budget and needs.


## Pages/Screens

- Landing/Home Page
- Login & Sign up Page
- Routine Page 
- Quiz Page
- Education Page

[Figma Wireframe](https://www.figma.com/design/cSHG9IziunARHO9NsmguJ2/dreamskin-wireframe?node-id=29-9787&t=w9egU63p7K9EW1GW-1)

## Data Model

Describe your app's data model using diagrams or tables

[Model Diagram](https://dbdiagram.io/d/dreamskin-data-model-669058ca9939893daeb5f9e5)

[Document of Data Model](https://docs.google.com/document/d/1RT-Y2oao9LKoy79ZWnIMXvj2X8ZostfqxqFoGwwCtVQ/edit)

## Endpoints

List the API endpoints you will need to implement.

## User Endpoints

1) Create User
    POST /users
    Creates a new user with the specified username, email, password, and skinType.
2) Get User by Username
    GET /users/:username
    Retrieves user details by their username.
3) Update User
    PUT /users/:username
    Updates the skinType, concerns and goals for the user identified by username
4) Delete User
    DELETE /users/:username
    Deletes the user account identified by username.

## Product Endpoints

1) Create Product
    POST /products
    Creates a new product with attributes including name, description, price, ingredients, and bestSkinType.
2) Get All Products
    GET /products
    Retrieves a list of all products available in the database.
3) Get Product by ID
    ET /products/:id
    Retrieves product details by its unique identifier (id).
4) Search Products by Ingredients
    ET /products-by-ingredients?ingredients=:ingredients
    It queries the local database to find products that contain any of the specified ingredients provided in the ingredients query parameter
5) Update Product
    PUT /products/:id
    Updates product details identified by id. Allows modifying name, description, price, ingredients, and bestSkinType.
6) Delete Product
    DELETE /products/:id
    Deletes the product identified by its unique id

## API Integration Endpoints
1) Fetch Recommended Ingredients
    GET /api/recommended-ingredients?skinType=:skinType
    Calls an external API to fetch recommended ingredients suitable for a specific skinType, concern, and goal.



***Don't forget to set up your Issues, Milestones, and Project Board!***
