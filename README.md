# Django Auctions

## Objetive
Build a system to manage auctions and lots and a public endpoint to query the auction details data given an auction id.

## Requirements
1. Create a new django app called ``auctions``
1. Add the models to represent auctions and lots.
For the auctions we need to be able to capture the name (required and max 150 characters), description (not required) and start date and time for the auction (required), Also we need to store the lots or items that are to sell in an auction event. For the lots we will need to capture the name of the item (required and max 150 characteres), the description (not required), and the starting sale price (required and we need a maximum of 10 digitis including 2 decimals). Ideally we would be able to query the lots from an auction instance like this ``auction_instance.lots.all()`` and the auction for a particular lot as follows ``lot_instance.auction()``
1. This models should be managed from the django admin section. 
1. Build a public endpoint to get the sale detail data including it's related lots. ie: ``/auctions/1/``
1. Add the logic needed to amend the data returned in the endpoint so the lot price includes VAT (20%)
1. Add tests (what do you think it'd be good to test)

#### Bonus points
1. Add to the models ``created`` and ``updated`` fields, using inherintance.
1. Config the admin so we can manage lots from the Auction details page.
2. Add crud endpoints for the auction resource
