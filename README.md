# UUIDBatch

UUIDBatch generates batches of UUID's. Each Batch contains approximately 500 ids and the program overall creates 8,000,000 batches to send to a Mongo datbase. Each bathc is categorized by it's mongo id and whether it has been used or not already. If it has it has an additional property stating which micro service it was used in.

A model for each batch: 

{
  "_id":"block1",
 "used": true,
 "service":"tool service",
  "block": [
    "uuid1", 
    "uuid2", 
    "uuid3", 
    "uuid4",
    ...,
    "uuid25"
    ]
}


