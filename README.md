# Screening Project: Styline Web and Backend Developer Recruitment
- Fork the repository
- Create an ecommerce store according to the guidelines below using any web stack/framework you are comfortable with
- Complete the sections after the horizontal line in the README to provide instructions about how to install the depepndencies and run the project
- After you are done send a pull request to the original repository

#### Project Spec (implement as much as you can)
- Use Moltin API/SDK functionalities (https://moltin.com/docs/)
- API Keys/SDK Credentials are provided via email
- A test store is already configured and prepopulated with products and categories

##### Objectives (Basic)
- Implement a product list/grid page (having pagination is a plus)
- Each product item should show product name, product image (just one), sku, price, stock and category
- Products should be filtered by categories, stock availablability
- Products should be sorted by price
- Implement Customer Sign Up and Login functionalities using Moltin SDK (No email/sms verification is required)
- If the customer is logged in, show customer's name and logout button.
- Also an add to cart button should be visible with each products if customer is logged in (and if the product is in stock)

##### Objectives (Advanced)
- Show a Cart button when customer is logged in
- If Add to cart is pressed the product should be added to cart
- Tapping the cart button should take the user to a cart page where all items in the cart should be listed
- User should be able to remove items from cart and go back to the product page from the cart page

##### Notes
- UI can be very simple, but should be consistent
- Any UI Framework/icon sets/themes can be used
- You must use the provided backend (Moltin) using any of their SDKs or REST API and have to use the API/Access Keys that has been provided
- Focus should be on workable and consistent functionalities rather than aesthetics

---
**Note**: Fill up the following sections before creating the pull request

<p align="center">
  <a href="https://ilovelamp.now.sh">
    <img src="https://i.imgur.com/B1EZxsB.png" alt="Moltin React Demo Store" />
  </a>
</p>

# Moltin &mdash; React Demo Store

An example store built using [React](https://reactjs.org/), [Redux](https://redux.js.org/) and [moltin](https://moltin.com). This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).

* [Demo](https://ilovelamp.now.sh)
* [API Reference](https://docs.moltin.com)

## Development

```bash
git clone https://github.com/moltin/react-demo-store.git
cd react-demo-store
yarn # or npm install
yarn start # or npm start
```

Note: You will want to change the `client_id` inside `src/moltin.js` with your own moltin store credentials.

This demo store uses the Redux "[ducks](https://github.com/erikras/ducks-modular-redux)" approach to bundling reducers and actions.

## Deployment

### Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

### Docker

1. [Download and install docker](https://docs.docker.com/engine/installation/)
2. Make sure docker is running locally
3. Run `docker build -t lamp .` at command line
4. Run the docker image with the command `docker run -p 5000 IMAGE_ID` where `IMAGE_ID` is the image ID shown in the result of step 3.
5. Access your app on port 5000

## Using this app with your own moltin store

The app expects a certain inventory setup to correctly function as an ILoveLamp store, if you'd like to build it from the ground up, here's what to do:

1. [Create a collection](https://docs.moltin.com/collection#create-a-collection) with the slug `top_picks`
2. [Create at least one category](https://docs.moltin.com/collection#create-a-category)
3. [Create at least one product](https://docs.moltin.com/collection#create-a-product)
4. [Create at least one file i.e. an image for your product](https://docs.moltin.com/collection#create-a-file)
5. [Attach the product/s to the category and collection](https://docs.moltin.com/collection#create-category-relationship-s-)
6. [Attach the file to the product as a main image](https://docs.moltin.com/collection#create-file-relationship-s-)
