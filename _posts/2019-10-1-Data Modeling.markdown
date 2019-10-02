---
layout: post
title:  Data Modeling
---
Author: Silas Myane
# Draw-Io & Vertabelo
This post is about my first experience making a data structure using Draw-Io and Vertabelo.
Draw-Io is the most tightly Google Drive integrated diagramming application available. draw.io. (6961) Works with. draw.io is completely free online diagram editor built around Google Drive(TM), that enables you to create flowcharts, UML, entity relation, network diagrams, mockups and more. Vertabelo is a visual database design tool available through a web browser. Vertabelo is a visual database design tool available through a web browser. It supports only the physical data modeling. We were tasked with creating a database diagram for this problem. An auction website has items for sale that are provided by sellers. Each item has an opening price, a description, and an ending time. Customers submit bids. The highest, earliest bid submitted before the ending time is the winning bid and the item is sold to the bidder. Each seller must pay the auction company 5% of the winning bid. The auction company wants to be able to analyze the sales behavior of its customers and sellers and so must keep track of all bids and sales.
# Draw-Io
<img src="{{ '/assets/img/Auction.jpg' | prepend: site.baseurl }}" alt="">
For my Draw-Io diagram I designed it based of the logic that made since to me and solved the problem. Basically a bidder can pick an item and then once a seller has selected an item they can place a bid on that item. Then that bid is stored in another table of all the information about the bid, seller, and buyer. Also a seller can create a new item to be auctioned off by giving it a opening price a brief description and a time that bidding can end.
# Vertabelo
<img src="{{ '/assets/img/house.png' | prepend: site.baseurl }}" alt="">
For my Vertabelo diagram I used my simple Draw-Io diagram as a templet for my more advanced diagram. A seller can be created by just giving a simple name, and they are assigned a PK. Then once someone has an account they can put an item up for auction. They must give the basic information as described in the problem, but the data base will also transfer the sellers id into the items data base as well. Then a Buyer can enter their name and be assigned a PK by the database. Then they can place a bid on an item. Then once the ending time has ran out the records of the bids on an item and who placed them will be stored in a separate table.
# Am I Satisfied?
I think my database would work but I am not 100% positive that the database to store all the information about the transactions that happen will.
