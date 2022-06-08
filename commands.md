# Put items

aws dynamodb put-item --table-name demo --item file://items/user1.json --return-consumed-capacity TOTAL --return-item-collection-metrics SIZE   

# Batch items
aws dynamodb batch-write-item --request-items file://items/users.json --return-consumed-capacity INDEXES --return-item-collection-metrics SIZE   
aws dynamodb batch-write-item --request-items file://items/wallets.json --return-consumed-capacity INDEXES --return-item-collection-metrics SIZE   