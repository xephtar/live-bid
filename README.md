
# Live BID

The purpose of the application is:

- [x] User can list item categories
- [x] User can see items in selected category
- [x] The list of items in screen will be updated if the new item created for that category or existed one is updated.
- [x]  User can list bids of item when expand the item
- [x]  User can offer a bid with the mail and amount
- [ ] The auction must be concluded after a certain time.
- [ ] Users should be notified by the e-mail entered.
- [ ] The winner of the auction should be decided who gives the most amount bid
- [ ] The winner of the auction should be sent a link to purchase the product.
  
 ## The API
 
API: [here](https://github.com/xephtar/live-bid-api)

- Used Neo4j as database
- Used Django as framework
- Used channels for websocket

Detailed instruction is in [readme](https://github.com/xephtar/live-bid-api/blob/main/README.md) file to run

 ## The UI
 
 UI: [here](https://github.com/xephtar/live-bid-ui)
 
 - Used Vue3

Detailed instruction is in [readme](https://github.com/xephtar/live-bid-ui/blob/main/README.md) file to run

 
 ## To create a scenario
 
You should use given [postman collection](https://github.com/xephtar/live-bid/blob/main/live-bid.postman_collection.json) in this repo after run the API project.

### Basic scenario
- Create a category or more
- Create an item with a category or more
- Create a bid for an item or more
- Open UI select category from drop down and get
- You can expand the item with clicking on it
- You can see list of bids if there are bids for that expanded item
- You can offer another bid

### Live item create scenario
- Create a category
- Open UI select the category and get
- Create an item for selected category
- Created item should be appeared in screen without refreshing

### Live item update scenario
- Create a category
- Create an item for selected category
- Open UI select the category and get
- Update the item
- The existed item in the screen should be updated with given new values


