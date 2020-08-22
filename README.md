# GoldEconomy
 Allows for a player ran gold-economy
 
 **Plugin created for specific server use, not generalised code for any server**
 
 A players balance is based off of how many gold ingots they have, as gold ingots are used as currency
 
 When a player sells an item, they choose how many of a particular item to sell and for how much
 
 When players buy from the market, they always buy the cheapest cost of the amount they want, so essentially the market is 'cheapest to sell x item gets it sold first'
 
 For example: '/sell 1 apple 1' Sells 1 apple for 1 gold ingot. This then removes the apple from your inventory.
 
 If a player wants to buy they type '/buy 1 apple 2' and this would buy the cheapest apple available on the market, if there is 1 apple available cheaper than the spending limit '2' typed in this command. This would then give the player who sold the apple 1 gold (the amount they sold it for) and the player who bought the item the 1 apple.
 
 If there are multiple players that you end up purchasing from, this distributes the gold appropriately to each player who sold items, for the amount they sold those items for,   and removes those items from the market appropriately.
 
There are no floating point errors due to use of BigDecimal and only truncating the result once showing it. Any financial calculations modify its reference to BigDecimal to maintain accuracy.
 
 This accounts for most items, besides any items that were illegal to be put on the shop, and also gives aliases for some items, such as potions for easy trading. 
